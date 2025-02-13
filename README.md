<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Experiência Única</title>
  <style>
    /* Estilização básica */
    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #74ebd5, #ACB6E5);
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      color: #333;
      transition: background 0.5s ease;
    }
    
    h1 {
      font-size: 2.5em;
      margin-bottom: 10px;
    }
    
    p {
      font-size: 1.1em;
      margin-bottom: 20px;
    }
    
    input {
      padding: 10px;
      font-size: 1em;
      border: none;
      border-radius: 5px;
      margin-bottom: 10px;
      outline: none;
    }
    
    button {
      padding: 10px 20px;
      font-size: 1em;
      border: none;
      border-radius: 5px;
      background-color: #333;
      color: #fff;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
    
    button:hover {
      background-color: #555;
    }
    
    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <h1 id="welcomeMessage">Bem-vindo(a)!</h1>
  <p id="userPrompt">Digite seu nome para personalizar sua experiência:</p>
  <input type="text" id="userName" placeholder="Seu nome" />
  <button id="submitBtn">Enviar</button>

  <script>
    // Seleciona os elementos do DOM
    const submitBtn = document.getElementById('submitBtn');
    const userNameInput = document.getElementById('userName');
    const welcomeMessage = document.getElementById('welcomeMessage');
    const userPrompt = document.getElementById('userPrompt');

    // Evento ao clicar no botão
    submitBtn.addEventListener('click', () => {
      const name = userNameInput.value.trim();
      if (name) {
        // Atualiza a mensagem de boas-vindas com o nome do usuário
        welcomeMessage.textContent = `Olá, ${name}! Seja bem-vindo(a)!`;
        userPrompt.textContent = `Que tal explorar nossa experiência personalizada?`;
        // Altera o fundo para dar um toque visual diferente
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
