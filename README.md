<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Animação de Gráfico de Barras</title>
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
      width: 0;
      line-height: 25px;
      text-align: right;
      padding-right: 10px;
      color: #fff;
      border-radius: 5px;
      /* A animação utiliza a propriedade customizada --progress */
      animation: progress 2s ease-out forwards;
    }
    /* Cores para cada tecnologia */
    .php         { background-color: #777BB4; }
    .javascript  { background-color: #F7DF1E; color: #000; }
    .csharp      { background-color: #239120; }
    .dart        { background-color: #0175C2; }
    .flutter     { background-color: #02569B; }
    .html5       { background-color: #E34F26; }
    .css3        { background-color: #1572B6; }

    @keyframes progress {
      from { width: 0; }
      /* A largura final é definida via propriedade customizada --progress */
      to { width: var(--progress); }
    }
  </style>
</head>
<body>
  <div class="skill">
    <h3>PHP (70%)</h3>
    <div class="progress-container">
      <div class="progress-bar php" style="--progress: 70%;"></div>
    </div>
  </div>

  <div class="skill">
    <h3>JavaScript (80%)</h3>
    <div class="progress-container">
      <div class="progress-bar javascript" style="--progress: 80%;"></div>
    </div>
  </div>

  <div class="skill">
    <h3>C# (60%)</h3>
    <div class="progress-container">
      <div class="progress-bar csharp" style="--progress: 60%;"></div>
    </div>
  </div>

  <div class="skill">
    <h3>Dart (70%)</h3>
    <div class="progress-container">
      <div class="progress-bar dart" style="--progress: 70%;"></div>
    </div>
  </div>

  <div class="skill">
    <h3>Flutter (70%)</h3>
    <div class="progress-container">
      <div class="progress-bar flutter" style="--progress: 70%;"></div>
    </div>
  </div>

  <div class="skill">
    <h3>HTML5 (90%)</h3>
    <div class="progress-container">
      <div class="progress-bar html5" style="--progress: 90%;"></div>
    </div>
  </div>

  <div class="skill">
    <h3>CSS3 (80%)</h3>
    <div class="progress-container">
      <div class="progress-bar css3" style="--progress: 80%;"></div>
    </div>
  </div>
</body>
</html>
