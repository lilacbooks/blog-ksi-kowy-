<!DOCTYPE html>
<html lang="pl">
<head>
  <meta charset="UTF-8">
  <title>lilac._.books</title>
  <style>
    body {
      margin: 0;
      font-family: 'Times New Roman', serif;
      background: linear-gradient(#f2e9ff, #e6d9ff);
      color: #4a356e;
    }

    header {
      text-align: center;
      padding: 40px 20px;
      font-size: 42px;
      font-weight: bold;
      letter-spacing: 2px;
    }

    header span {
      font-size: 18px;
      display: block;
      margin-top: 10px;
      color: #7a5fa3;
    }

    nav {
      display: flex;
      justify-content: center;
      gap: 20px;
      background: #d8c7ff;
      padding: 15px;
    }

    nav button {
      background: #f7f2ff;
      border: none;
      padding: 10px 25px;
      border-radius: 20px;
      font-weight: bold;
      cursor: pointer;
      color: #5b3f88;
      transition: 0.3s;
    }

    nav button:hover {
      background: #cbb6ff;
    }

    .content {
      max-width: 900px;
      margin: auto;
      padding: 40px 20px;
    }

    .post {
      background: #fff;
      padding: 25px;
      margin-bottom: 25px;
      border-radius: 18px;
      box-shadow: 0 0 15px rgba(120, 90, 180, 0.15);
    }

    .post h2 {
      color: #6a4fa3;
    }

    .post img {
      max-width: 100%;
      border-radius: 12px;
      margin-top: 15px;
    }

    .hidden {
      display: none;
    }

    footer {
      text-align: center;
      padding: 30px;
      font-size: 14px;
      color: #7a5fa3;
    }
  </style>
</head>

<body>

<header>
  lilac._.books  
  <span>fantasy • romance • cozy reads</span>
</header>

<nav>
  <button onclick="showSection('nowe')">Nowe</button>
  <button onclick="showSection('recenzje')">Recenzje</button>
</nav>

<div class="content">

  <!-- ➕ Tu wklejasz nowe książki -->
  <div id="nowe">
    <div class="post">
      <h2>✨ Aktualnie czytam</h2>
      <p>„Fourth Wing” – smoki, magia i dramat. Już wiem, że będę obsesyjna.</p>
      <!-- Przykład zdjęcia książki -->
      <!-- <img src="images/fourthwing.jpg" alt="Fourth Wing"> -->
    </div>
  </div>

  <!-- ➕ Tu wklejasz recenzje -->
  <div id="recenzje" class="hidden">
    <div class="post">
      <h2>💜 Recenzja: „It Ends With Us”</h2>
      <p>Emocjonalny rollercoaster. Delikatna, bolesna i piękna historia. 9/10.</p>
      <!-- <img src="images/itendswithus.jpg" alt="It Ends With Us"> -->
    </div>
  </div>

</div>

<footer>
  © lilac._.books • made with magic ✨
</footer>

<script>
  function showSection(section) {
    document.getElementById('nowe').classList.add('hidden');
    document.getElementById('recenzje').classList.add('hidden');
    document.getElementById(section).classList.remove('hidden');
  }
</script>

</body>
</html>
