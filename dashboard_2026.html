const csvLinks = {
  A: "https://docs.google.com/spreadsheets/d/e/2PACX-1vSOuipD2-NGSfsSNYmZtQiaOyxCrTGMUhdXXbTfOeP46d53qe7jLaCzgWp-hYw4_A/pub?gid=1397944008&single=true&output=csv"
};

function openCard(cardId) {

  const csvUrl = csvLinks[cardId];

  if (!csvUrl) {
    alert("CSV link not found");
    return;
  }

  Papa.parse(csvUrl, {
    download: true,
    header: true,

    complete: function(results) {

      console.log(results.data);

      let tableHTML = `
        <html>
        <head>
        <title>2025-2026</title>

        <style>

        body{
          font-family:Arial;
          padding:20px;
          background:#f4f4f4;
        }

        table{
          width:100%;
          border-collapse:collapse;
          background:white;
        }

        th,td{
          border:1px solid #ccc;
          padding:10px;
          text-align:left;
        }

        th{
          background:#4CAF50;
          color:white;
        }

        </style>
        </head>
        <body>

        <h2>2025-2026</h2>
        <table>
      `;

      const headers = Object.keys(results.data[0]);

      tableHTML += "<tr>";

      headers.forEach(header => {
        tableHTML += `<th>${header}</th>`;
      });

      tableHTML += "</tr>";

      results.data.forEach(row => {

        tableHTML += "<tr>";

        headers.forEach(header => {
          tableHTML += `<td>${row[header] || ""}</td>`;
        });

        tableHTML += "</tr>";
      });

      tableHTML += "</table></body></html>";

      const newWindow = window.open();

      newWindow.document.write(tableHTML);

    },

    error: function(error) {
      console.error(error);
      alert("Unable to load CSV data");
    }

  });

}
