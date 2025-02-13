<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Experiência Única</title>
  <style>
    /* Importa a fonte Montserrat do Google Fonts */
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
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      background: linear-gradient(135deg, #89f7fe, #66a6ff);
      transition: background 1s ease-in-out;
    }

    h1 {
      font-size: 3em;
      color: #fff;
      margin-bottom: 20px;
      text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.3);
      animation: fadeInDown 1s ease-out;
    }

    p {
      font-size: 1.2em;
      color: #f0f0f0;
      margin-bottom: 20px;
      animation: fadeIn 1s ease-out;
    }

    input {
      padding: 15px;
      font-size: 1em;
      border: none;
      border-radius: 50px;
      outline: none;
      margin-bottom: 20px;
      width: 250px;
      text-align: center;
      transition: transform 0.3s ease;
    }

    input:focus {
      transform: scale(1.05);
    }

    button {
      padding: 15px 30px;
      font-size: 1em;
      border: none;
      border-radius: 50px;
      background-color: #fff;
      color: #333;
      cursor: pointer;
      transition: background-color 0.3s ease, transform 0.3s ease;
      box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
    }

    button:hover {
      background-color: #f0f0f0;
      transform: scale(1.05);
    }

    .hidden {
      display: none;
    }

    /* Animações */
    @keyframes fadeInDown {
      0% {
        opacity: 0;
        transform: translateY(-20px);
      }
      100% {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
  </style>
</head>
<body>
  <h1 id="welcomeMessage">Bem-vindo(a)!</h1>
  <p id="userPrompt">Digite seu nome para personalizar sua experiência:</p>
  <input type="text" id="userName" placeholder="Seu nome" />
  <button id="submitBtn">Enviar</button>

  <script>
    const submitBtn = document.getElementById('submitBtn');
    const userNameInput = document.getElementById('userName');
    const welcomeMessage = document.getElementById('welcomeMessage');
    const userPrompt = document.getElementById('userPrompt');

    submitBtn.addEventListener('click', () => {
      const name = userNameInput.value.trim();
      if (name) {
        welcomeMessage.textContent = `Olá, ${name}! Seja bem-vindo(a)!`;
        userPrompt.textContent = `Explore nossa experiência personalizada.`;
        // Altera o fundo para um novo gradiente
        document.body.style.background = "linear-gradient(135deg, #f6d365, #fda085)";
        // Esconde o campo de input e o botão após o envio
        userNameInput.classList.add('hidden');
        submitBtn.classList.add('hidden');
      } else {
        alert('Por favor, digite seu nome.');
      }
    });
  </script>
</body>
</html>
