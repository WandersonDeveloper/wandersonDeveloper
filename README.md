<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Experiência Única - Apenas HTML & CSS</title>
  <style>
    /* Importa a fonte Montserrat */
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&display=swap');

    /* Reset básico */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Montserrat', sans-serif;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      background: linear-gradient(135deg, #89f7fe, #66a6ff);
      transition: background 0.5s ease;
    }

    .container {
      text-align: center;
      color: #fff;
      padding: 20px;
      border-radius: 10px;
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 20px;
    }

    p {
      font-size: 1.2rem;
      margin-bottom: 20px;
    }

    /* Esconde o checkbox */
    #toggle {
      display: none;
    }

    /* Estilo do botão (label) */
    .label-button {
      display: inline-block;
      padding: 15px 30px;
      font-size: 1rem;
      border-radius: 50px;
      background: #fff;
      color: #333;
      cursor: pointer;
      transition: background 0.3s ease, transform 0.3s ease;
      box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
    }

    .label-button:hover {
      background: #f0f0f0;
      transform: scale(1.05);
    }

    /* Estado alternado: quando o checkbox está marcado */
    #toggle:checked ~ .container {
      background: linear-gradient(135deg, #f6d365, #fda085);
      box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.3);
    }

    /* Conteúdo adicional inicialmente oculto */
    .toggled-message {
      opacity: 0;
      max-height: 0;
      overflow: hidden;
      transition: opacity 0.5s ease, max-height 0.5s ease;
    }

    /* Exibe o conteúdo quando o checkbox está marcado */
    #toggle:checked ~ .container .toggled-message {
      opacity: 1;
      max-height: 200px;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <!-- Checkbox oculto para controlar o estado -->
  <input type="checkbox" id="toggle">
  
  <div class="container">
    <h1>Bem-vindo(a)!</h1>
    <p>Clique no botão para personalizar sua experiência.</p>
    <!-- Label atuando como botão -->
    <label for="toggle" class="label-button">Ativar Experiência</label>
    
    <!-- Conteúdo que aparece quando ativado -->
    <div class="toggled-message">
      <p>Experiência personalizada ativada!</p>
      <p>Aproveite a nova aparência e estilo.</p>
    </div>
  </div>
</body>
</html>
