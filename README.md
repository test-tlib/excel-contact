<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Excel Upload & Parse</title>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
  <style>
    .drop-zone {
      border: 2px dashed #ccc;
      padding: 30px;
      text-align: center;
      margin: 20px;
      cursor: pointer;
    }
  </style>
</head>
<body class="p-4">
  <h2>Upload Excel or CSV</h2>

  <div id="drop-zone" class="drop-zone">Drag & Drop file here or click to upload</div>
  <input type="file" id="file-input" accept=".xlsx,.csv" class="form-control mt-2" />

  <h4 class="mt-4">Parsed Contacts</h4>
  <table class="table table-bordered mt-2" id="preview-table">
    <thead>
      <tr><th>Name</th><th>Number</th><th>Message</th></tr>
    </thead>
    <tbody></tbody>
  </table>

  <h4>Generated JSON</h4>
  <pre id="json-output" style="background:#f8f8f8; padding:10px; border:1px solid #ccc;"></pre>
k below]
