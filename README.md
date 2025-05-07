# Day3-LeProject
A site with 3 img and stuff:
is not structured but idk how to save the code yet... ye so here it is copy it then try to glue it all together


<!DOCTYPE html>
<html lang="ro">
<head>
  <meta charset="UTF-8">
  <title>Proiect de initiere Rc-241</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      font-family: Arial, sans-serif;
    }

    body {
      display: flex;
      flex-direction: column;
    }

    .navbar {
      background-color: #007BFF;
      color: white;
      padding: 10px;
      text-align: center;
      position: relative;
    }

    .navbar .corner-left {
      position: absolute;
      top: 10px;
      left: 10px;
      font-size: 12px;
      font-weight: bold;
    }

    .navbar .corner-right {
      position: absolute;
      top: 10px;
      right: 10px;
      font-size: 12px;
      font-weight: bold;
    }

    .section {
      flex: 1;
      padding: 20px;
      text-align: center;
    }

    .row {
      display: flex;
      justify-content: center;
      gap: 20px;
      flex-wrap: wrap;
      margin: 20px 0;
    }

    .img-box {
      width: 250px;
      height: 250px;
      background-color: #4a90e2;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .img-box img {
      max-width: 100%;
      max-height: 100%;
      object-fit: cover;
    }

    input[type="text"], input[type="date"], select {
      padding: 5px;
    }

    .circle {
      width: 20px;
      height: 20px;
      border: 2px solid black;
      border-radius: 50%;
      display: inline-block;
      margin-right: 10px;
      vertical-align: middle;
      cursor: pointer;
    }

    .circle.filled {
      background-color: black;
    }

    .square {
      width: 20px;
      height: 20px;
      border: 2px solid black;
      display: inline-block;
      margin-right: 10px;
      vertical-align: middle;
      cursor: pointer;
    }

    .square.checked {
      background-color: #4a90e2;
      background-image: url('data:image/svg+xml;utf8,<svg fill="white" viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg"><path d="M6.173 13.207l-4.24-4.24L3.6 7.3l2.573 2.573L12.4 3.646l1.414 1.415z"/></svg>');
      background-repeat: no-repeat;
      background-position: center;
      background-size: 14px;
    }

    .footer {
      background-color: #007BFF;
      color: white;
      padding: 20px 0;
      position: relative;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .footer .corner-left {
      position: absolute;
      bottom: 10px;
      left: 10px;
      font-size: 12px;
      font-weight: bold;
    }

    .footer .corner-right {
      position: absolute;
      bottom: 10px;
      right: 10px;
      font-size: 12px;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <div class="navbar">
    <div class="corner-left">CristianS</div>
    <div class="corner-right">CristianS</div>
    <strong>Proiect de initiere Rc-241</strong>
  </div>

  <div class="section">
    <!-- Form section -->
    <div class="row">
      <input type="text" placeholder="Introdu textul aici">
      <select>
        <option value="">Alege...</option>
        <option value="important">Important</option>
        <option value="mediu">Mediu</option>
      </select>
      <input type="date">
    </div>

    <!-- Image section -->
    <div class="row">
      <div class="img-box"><img src="https://4kwallpapers.com/images/walls/thumbs_3t/14884.jpg" alt="Imagine 1"></div>
      <div class="img-box"><img src="https://images2.alphacoders.com/137/1372963.png" alt="Imagine 2"></div>
      <div class="img-box"><img src="https://images4.alphacoders.com/137/1374662.png" alt="Imagine 3"></div>
    </div>

    <!-- Text sections -->
    <div class="row" style="margin-top: 20px;">
      <div class="circle" onclick="toggleCircle(this)"></div>
      <span>Varianta Corecta</span>
    </div>

    <div class="row" style="margin-top: 20px;">
      <div class="square" onclick="toggleSquare(this)"></div>
      <span>Raspuns Corect</span>
    </div>
  </div>

  <!-- Footer -->
  <div class="footer">
    <div class="corner-left">CristianS</div>
    <div class="corner-right">CristianS</div>
     2025 Proiect RC-241
  </div>

  <script>
    function toggleCircle(elem) {
      elem.classList.toggle('filled');
    }

    function toggleSquare(elem) {
      elem.classList.toggle('checked');
    }
  </script>

</body>
</html>
