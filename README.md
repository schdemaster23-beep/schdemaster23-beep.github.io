# schdemaster23-beep.github.io
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Автор Щуренко Д Э | Поэзия Души</title>

  <style>
    body {
      margin: 0;
      font-family: Georgia, serif;
      background: #f4f4f4;
      color: #222;
    }

    header {
      background: #1e1e1e;
      color: white;
      padding: 20px;
      text-align: center;
    }

    nav {
      display: flex;
      justify-content: center;
      background: #333;
    }

    nav button {
      background: none;
      border: none;
      color: white;
      padding: 15px 20px;
      font-size: 16px;
      cursor: pointer;
    }

    nav button:hover {
      background: #555;
    }

    nav button.active {
      background: #111;
    }

    .content {
      max-width: 800px;
      margin: 30px auto;
      background: white;
      padding: 25px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    .tab {
      display: none;
    }

    .tab.active {
      display: block;
    }

    h2 {
      text-align: center;
    }

    .poem {
      white-space: pre-line;
      line-height: 1.6;
      margin-top: 20px;
    }

    footer {
      text-align: center;
      padding: 15px;
      font-size: 14px;
      color: #666;
    }
  </style>
</head>

<body>

<header>
  <h1>Автор Щуренко Д Э | Поэзия Души</h1>
  <p>Поэзия и произведения</p>
</header>

<nav>
  <button class="active" onclick="openTab('about')">Об авторе</button>
  <button onclick="openTab('poems')">Стихи</button>
  <button onclick="openTab('works')">Произведения</button>
</nav>

<div class="content">

  <div id="about" class="tab active">
    <h2>Об авторе</h2>
    <p>
      Я — автор, поэт, человек слова.  
      Здесь собраны мои стихи и произведения,  
      написанные в разное время и разным состоянием души.
    </p>
  </div>

  <div id="poems" class="tab">
    <h2>Стихи</h2>

    <div class="poem">
тут будет много мыслей и стих стихи 
    </div>

    <hr>

    <div class="poem">
ничего не понятно но очень интересно 
    </div>
  </div>

  <div id="works" class="tab">
    <h2>Произведения</h2>
    <p><b>Название:</b> Тени между строк</p>
    <p>
      ге человека.
    </p>
  </div>

</div>

<footer>
  © 2026 | Авторские права
</footer>

<script>
  function openTab(tabId) {
    const tabs = document.querySelectorAll('.tab');
    const buttons = document.querySelectorAll('nav button');

    tabs.forEach(tab => tab.classList.remove('active'));
    buttons.forEach(btn => btn.classList.remove('active'));

    document.getElementById(tabId).classList.add('active');
    event.target.classList.add('active');
  }
</script>

</body>
</html>
