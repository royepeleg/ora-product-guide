---
title: "Technical data"
---

# Product Specifications

Below is the full technical specification of the product.

<link rel="stylesheet" href="https://cdn.datatables.net/1.13.7/css/jquery.dataTables.min.css">

<script src="https://code.jquery.com/jquery-3.7.1.min.js"></script>
<script src="https://cdn.datatables.net/1.13.7/js/jquery.dataTables.min.js"></script>

<table id="specTable" class="display" style="width:100%; margin-top: 20px;">
  <thead>
    <tr>
      <th>Parameter</th>
      <th>Value</th>
      <th>Units</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
  </tbody>
</table>

<script>
async function loadSpecs() {
  try {
    const response = await fetch('/data/BOM.csv');
    const text = await response.text();

    // Split into rows
    let rows = text.trim().split('\n').map(r => r.split(',').map(c => c.trim()));

    // Remove empty rows (all columns empty)
    rows = rows.filter(row => row.some(cell => cell !== ""));

    // Transpose to detect empty columns
    const columns = rows[0].length;
    const columnIsEmpty = Array(columns).fill(true);

    for (let col = 0; col < columns; col++) {
      for (let row = 0; row < rows.length; row++) {
        if (rows[row][col] && rows[row][col].trim() !== "") {
          columnIsEmpty[col] = false;
          break;
        }
      }
    }

    // Build the final filtered table
    const filteredRows = rows.map(row =>
      row.filter((_, colIndex) => !columnIsEmpty[colIndex])
    );

    const tbody = document.querySelector('#specTable tbody');

    // Skip header row when inserting HTML table body
    for (let i = 1; i < filteredRows.length; i++) {
      const tr = document.createElement('tr');
      filteredRows[i].forEach(col => {
        const td = document.createElement('td');
        td.innerText = col;
        tr.appendChild(td);
      });
      tbody.appendChild(tr);
    }

    // Replace table headers to match filtered columns
    const headerRow = document.querySelector('#specTable thead tr');
    headerRow.innerHTML = "";
    filteredRows[0].forEach(header => {
      const th = document.createElement('th');
      th.innerText = header;
      headerRow.appendChild(th);
    });

    // Activate DataTables
    $('#specTable').DataTable();
  } catch (err) {
    console.error("Error loading specs:", err);
  }
}

loadSpecs();
</script>
