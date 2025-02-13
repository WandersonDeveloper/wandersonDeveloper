<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Página com Tinah Fito</title>
  <style>
    /* Reset básico */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      background: #f4f4f4;
      color: #333;
    }

    /* Header com banner */
    header {
      position: relative;
      width: 100%;
      height: 300px;
      background: url('https://via.placeholder.com/1200x300?text=Tinah+Fito') no-repeat center center;
      background-size: cover;
    }

    /* Sobreposição para melhor contraste */
    header .overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.5);
    }

    header h1 {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      color: #fff;
      font-size: 3rem;
      text-align: center;
      z-index: 1;
    }

    /* Conteúdo principal */
    main {
      padding: 20px;
    }

    .content {
      max-width: 800px;
      margin: 0 auto;
      background: #fff;
      padding: 20px;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    .content h2 {
      margin-bottom: 15px;
    }

    .content p {
      margin-bottom: 10px;
      text-align: justify;
    }
  </style>
</head>
<body>
  <header>
    <div class="overlay"></div>
    <h1>Tinah Fito</h1>
  </header>

  <main>
    <div class="content">
      <h2>Bem-vindo à minha página!</h2>
      <p>
        Esta é uma página de exemplo criada para o GitHub, com um banner impactante no início. 
        Você pode utilizar este template para mostrar seu portfólio, projetos ou qualquer outro conteúdo.
      </p>
      <p>
        Basta personalizar as imagens, textos e cores conforme sua identidade visual.
      </p>
    </div>
  </main>
</body>
</html>
