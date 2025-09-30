<!DOCTYPE html>
<html lang="fi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Self-Help-You</title>
  <style>
    /* Styling the navigation bar */
    .navbar {
      background-color: #e1705d;
      overflow: hidden;
      text-align: center;
    }

    .navbar a {
      display: inline-block;
      padding: 14px 20px;
      text-decoration: none;
      color: white;
      font-size: 14px;
      transition: background-color 0.3s ease;
    }

    .navbar a:hover {
      background-color: #ddd;
      color: black;
    }

    .navbar a.active {
      background-color: #0e194d;
      color: white;
    }

    .navbar .icon {
      z-index: 2;
      display: none;
      font-size: 27px;
      color: white;
      padding: 14px 20px;
      background-color: #0e194d;
      cursor: pointer;
    }

    @media screen and (max-width: 768px) {
      .navbar a {
        display: none;
        width: 100%;
        text-align: left;
        padding: 14px;
      }

      .navbar a.active {
        background-color: #0e194d;
        color: white;
      }

      .navbar .icon {
        display: block;
      }

      .navbar.responsive a {
        display: block;
      }

      .navbar.responsive .icon {
        position: absolute;
        right: 0;
        top: 0;
      }
    }

    .header {
      background-color: #0e194d;
      color: white;
      padding: 20px;
      text-align: center;
      position: relative;
      overflow: hidden;
    }

    .header h1 {
      display: inline-block;
      font-size: 27px;
      white-space: nowrap;
      animation: rollText 10s linear infinite;
      position: relative;
      z-index: 2;
    }

    @keyframes rollText {
      0% {
        transform: translateX(100%);
      }
      100% {
        transform: translateX(-100%);
      }
    }

    .intro-text {
      text-align: center;
      padding: 40px;
      background-color: #f0f0f0;
    }

    .intro-text h2 {
      font-size: 24px;
      color: #0e194d;
    }

    .intro-text p {
      font-size: 14px;
      color: #0e194d;
    }

    .box-container {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px;
      margin-top: 40px;
      padding: 0 20px;
    }

    .box-container .box-image {
      grid-column: span 2;
    }

    .box {
      background-color: #0e194d;
      box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3),
                  -2px -2px 5px rgba(92, 97, 102, 0.5);
      border: 1px solid #ddd;
      border-radius: 8px;
      text-align: center;
      padding: 20px;
      transition: transform 0.3s ease;
    }

    .box h3 {
      margin-bottom: 15px;
      font-size: 24px;
      text-shadow: 2px 2px 5px black;
      color: #0e194d;
    }

    .box p {
      font-size: 14px;
      color: #0e194d;
    }

    .box:hover {
      transform: translateY(-10px);
    }

    .box-small {
      background-image: url('Pallot.jpg');
      box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3),
                  -2px -2px 5px rgba(92, 97, 102, 0.5);
      padding: 20px;
      height: 150px;
      border-radius: 8px;
      text-align: center;
      transition: transform 0.3s ease;
      color: #0e194d;
    }

    .box-image {
      background-image: url('Kuva20.jpg');
      background-size: cover;
      background-position: center;
      color: #0e194d;
      padding: 40px;
      text-align: center;
      border-radius: 8px;
      box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3),
                  -2px -2px 5px rgba(92, 97, 102, 0.5);
    }

    .box-image h3 {
      margin-bottom: 20px;
      font-size: 24px;
      color: #e1705d;
    }

    .box-image p {
      font-size: 14px;
      color: #e1705d;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #0e194d;
      color: white;
    }

    footer a {
      text-decoration: none;
      color: white;
      font-size: 16px;
      margin: 0 10px;
      transition: color 0.3s ease;
    }

    footer a:hover {
      color: #FF5733;
    }

    footer a:visited {
      color: #8E44AD;
    }

    .footer-bottom {
      padding-top: 10px;
    }

    section {
      padding-bottom: 40px;
    }
  </style>
</head>
<body>

  <nav class="navbar" id="myNavbar">
    <a href="#" class="active">Etusivu</a>
    <a href="#">Palvelut</a>
    <a href="#">Koulutus</a>
    <a href="#">Yhteystiedot</a>
    <a href="javascript:void(0);" class="icon" onclick="toggleNavbar()">&#9776;</a>
  </nav>

  <header class="header">
    <h1>Tervetuloa Self-Help-You -palveluun!</h1>
  </header>

  <section class="intro-text">
    <h2>Me autamme sinua onnistumaan</h2>
    <p>Tarjoamme räätälöityjä konsultointipalveluita ja koulutuksia yrityksellesi.</p>
  </section>

  <section class="box-container">
    <div class="box-small box">
      <h3>Tarina</h3>
      <p>Yrityksemme tarina ja arvot</p>
    </div>
    <div class="box-small box">
      <h3>Palvelut</h3>
      <p>Tutustu tarjoamiimme palveluihin</p>
    </div>
    <div class="box-image">
      <h3>Koulutus</h3>
      <p>Koulutukset ja verkkokurssit</p>
    </div>
    <div class="box-image">
      <h3>Yhteystiedot</h3>
      <p>Ota yhteyttä ja kerro tarpeistasi</p>
    </div>
  </section>

  <footer>
    <div>
      <a href="#">Etusivu</a>
      <a href="#">Palvelut</a>
      <a href="#">Koulutus</a>
      <a href="#">Yhteystiedot</a>
    </div>
    <div class="footer-bottom">
      &copy; 2025 Self-Help-You. Kaikki oikeudet pidätetään.
    </div>
  </footer>

  <script>
    function toggleNavbar() {
      var x = document.getElementById("myNavbar");
      if (x.className === "navbar") {
        x.className += " responsive";
      } else {
        x.className = "navbar";
      }
    }
  </script>
</body>
</html>
