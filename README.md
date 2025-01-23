
<!-- interest table toggleable -->
<style>
  .custom-table {
    border-collapse: collapse;
    margin: 0px auto; /* Center horizontally and add vertical margin */
    width: 70%; /* Optional: adjust the width as needed */
    max-width: 800px; /* Optional: adjust the max-width as needed */
  }
  .custom-table th, .custom-table td {
    border: 1px solid #ddd;
    padding: 3px;
    height: 3px; /* Set height for rows */
  }
  .custom-table th {
    background-color: #f4f4f4;
    text-align: left;
  }
  
  .hidden {
    display: none;
  }
  #toggle-button {
    float: right; /* Float the button to the right */
  }
</style>

<button id="toggle-button" onclick="toggleTable()" style="font-size: 15px">See topic distribution</button>

<table id="interest-table" class="custom-table hidden">
  <thead>
    <tr>
      <th style="font-size: 15px">Research Topic</th>
      <th style="font-size: 15px">Topic distribution (Ph.D.)</th>
      <th style="font-size: 15px">Topic distribution (Postdoc)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="font-size: 15px">Recommender System</td>
      <td style="font-size: 15px">███████ 0.371</td>
      <td style="font-size: 15px">██ 0.108</td>
    </tr>
    <tr>
      <td style="font-size: 15px">Knowledge Distillation</td>
      <td style="font-size: 15px">██████ 0.314</td>
      <td style="font-size: 15px">██ 0.081</td>
    </tr>
    <tr>
      <td style="font-size: 15px">Model Compression</td>
      <td style="font-size: 15px">████ 0.172</td>
      <td style="font-size: 15px">█ 0.027</td>
    </tr>
    <tr>
      <td style="font-size: 15px">Ensemble Learning</td>
      <td style="font-size: 15px">███ 0.132</td>
      <td style="font-size: 15px">-</td>
    </tr>
    <tr>
      <td style="font-size: 15px">Document Retrieval</td>
      <td style="font-size: 15px">-</td>
      <td style="font-size: 15px">███████ 0.351</td>
    </tr>
    <tr>
      <td style="font-size: 15px">Large Language Model</td>
      <td style="font-size: 15px">-</td>
      <td style="font-size: 15px">█████ 0.243</td>
    </tr>
    <tr>
      <td style="font-size: 15px">Topic & Phrase Mining</td>
      <td style="font-size: 15px">-</td>
      <td style="font-size: 15px">████ 0.189</td>
    </tr>
  </tbody>
</table>

<script>
  function toggleTable() {
    var table = document.getElementById('interest-table');
    var button = document.getElementById('toggle-button');
    if (table.classList.contains('hidden')) {
      table.classList.remove('hidden');
      button.textContent = 'Hide topic distribution';
    } else {
      table.classList.add('hidden');
      button.textContent = 'See topic distribution';
    }
  }
</script>
<!-- interest table toggleable -->