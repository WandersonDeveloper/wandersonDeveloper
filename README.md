<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Gráfico de Barras Estático</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 20px;
      background: #f5f5f5;
    }
    .skill {
      margin-bottom: 20px;
    }
    .skill h3 {
      margin: 0 0 5px;
      font-size: 1rem;
    }
    .progress-container {
      width: 100%;
      background: #ddd;
      border-radius: 5px;
      overflow: hidden;
    }
    .progress-bar {
      height: 25px;
      line-height: 25px;
      text-align: right;
      padding-right: 10px;
      color: #fff;
      border-radius: 5px;
    }
    /* Define as cores e larguras estáticas para cada tecnologia */
    .php         { background-color: #777BB4; width: 70%; }
    .javascript  { background-color: #F7DF1E; color: #000; width: 80%; }
    .csharp      { background-color: #239120; width: 60%; }
    .dart        { background-color: #0175C2; width: 70%; }
    .flutter     { background-color: #02569B; width: 70%; }
    .html5       { background-color: #E34F26; width: 90%; }
    .css3        { background-color: #1572B6; width: 80%; }
  </style>
</head>
<body>
  <div class="skill">
    <h3>PHP (70%)</h3>
    <div class="progress-container">
      <div class="progress-bar php"></div>
    </div>
  </div>

  <div class="skill">
    <h3>JavaScript (80%)</h3>
    <div class="progress-container">
      <div class="progress-bar javascript"></div>
    </div>
  </div>

  <div class="skill">
    <h3>C# (60%)</h3>
    <div class="progress-container">
      <div class="progress-bar csharp"></div>
    </div>
  </div>

  <div class="skill">
    <h3>Dart (70%)</h3>
    <div class="progress-container">
      <div class="progress-bar dart"></div>
    </div>
  </div>

  <div class="skill">
    <h3>Flutter (70%)</h3>
    <div class="progress-container">
      <div class="progress-bar flutter"></div>
    </div>
  </div>

  <div class="skill">
    <h3>HTML5 (90%)</h3>
    <div class="progress-container">
      <div class="progress-bar html5"></div>
    </div>
  </div>

  <div class="skill">
    <h3>CSS3 (80%)</h3>
    <div class="progress-container">
      <div class="progress-bar css3"></div>
    </div>
  </div>
</body>
</html>
