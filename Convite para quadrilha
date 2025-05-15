<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Convite para Quadrilha</title>
<style>
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: linear-gradient(45deg, #fceabb, #f8b500);
    color: #4a2c00;
    display: flex;
    height: 100vh;
    margin: 0;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    text-align: center;
    padding: 1rem;
  }
  a.invite-link {
    font-size: 1.8rem;
    background: #d26100;
    color: #fff;
    padding: 1rem 2rem;
    border-radius: 40px;
    text-decoration: none;
    box-shadow: 0 8px 15px rgba(210, 97, 0, 0.4);
    transition: background 0.3s, box-shadow 0.3s;
    cursor: pointer;
  }
  a.invite-link:hover {
    background: #ffa632;
    box-shadow: 0 12px 20px rgba(255, 166, 50, 0.6);
  }
  .invitation-container {
    margin-top: 2rem;
    max-width: 380px;
    background: #fff3d0;
    border-radius: 15px;
    border: 2px solid #d26100;
    padding: 1.5rem;
    color: #663c00;
    box-shadow: 0 4px 10px rgba(210, 97, 0, 0.3);
  }
  .invitation-text {
    font-size: 1.2rem;
    white-space: pre-line;
    line-height: 1.4;
    margin-bottom: 1.5rem;
  }
  .response-buttons {
    display: flex;
    justify-content: center;
    gap: 1rem;
  }
  button {
    font-size: 1.1rem;
    padding: 0.6rem 1.5rem;
    border-radius: 30px;
    border: none;
    cursor: pointer;
    box-shadow: 0 5px 10px rgba(210, 97, 0, 0.4);
    transition: background 0.3s, box-shadow 0.3s;
  }
  button.sim {
    background-color: #28a745;
    color: #fff;
  }
  button.sim:hover {
    background-color: #5bd36f;
    box-shadow: 0 8px 15px rgba(91, 211, 111, 0.6);
  }
  button.nao {
    background-color: #dc3545;
    color: #fff;
  }
  button.nao:hover {
    background-color: #ef5b64;
    box-shadow: 0 8px 15px rgba(239, 91, 100, 0.6);
  }
</style>
</head>
<body>
  <a href="#" class="invite-link" id="inviteLink">💃 Convite para Quadrilha 💃</a>

  <div id="invitationContainer" class="invitation-container" style="display:none;">
    <div id="invitationText" class="invitation-text"></div>
    <div class="response-buttons" id="responseButtons">
      <button class="sim" id="btnSim">Sim</button>
      <button class="nao" id="btnNao">Não</button>
    </div>
  </div>

<script>
  // Helper to get URL parameter by name
  function getParameterByName(name) {
    const url = window.location.href;
    name = name.replace(/[\\[\\]]/g, '\\$&');
    const regex = new RegExp('[?&]' + name + '(=([^&#]*)|&|#|$)');
    const results = regex.exec(url);
    if (!results) return null;
    if (!results[2]) return '';
    return decodeURIComponent(results[2].replace(/\+/g, ' '));
  }

  // Get the "name" parameter or default "Bruna"
  const convidada = getParameterByName('name') || 'Bruna';

  const conviteTexto =
`🤠 Olá, ${convidada}! 🤠

Você aceita ser minha par no baile de quadrilha?
Prepare seu traje, seu sorriso e muita animação!

Será uma noite inesquecível com muita festa, dança e alegria!
Espero de coração seu SIM para formarmos a dupla mais animada do baile!

Com carinho,
Seu parceiro de dança 🕺

👢🎉 Vamos juntos arrasar na quadrilha! 🎉👢`;

  const inviteLink = document.getElementById('inviteLink');
  const invitationContainer = document.getElementById('invitationContainer');
  const invitationText = document.getElementById('invitationText');
  const responseButtons = document.getElementById('responseButtons');
  const btnSim = document.getElementById('btnSim');
  const btnNao = document.getElementById('btnNao');

  inviteLink.addEventListener('click', (e) => {
    e.preventDefault();
    if (invitationContainer.style.display === 'none') {
      invitationText.textContent = conviteTexto;
      invitationContainer.style.display = 'block';
      inviteLink.textContent = '❌ Fechar Convite';
    } else {
      invitationContainer.style.display = 'none';
      inviteLink.textContent = '💃 Convite para Quadrilha 💃';
      invitationText.textContent = '';
      responseButtons.style.display = 'flex';
    }
  });

  btnSim.addEventListener('click', () => {
    invitationText.textContent = '🎉 Que alegria! Mal posso esperar para dançarmos juntos! 🕺💃';
    responseButtons.style.display = 'none';
  });

  btnNao.addEventListener('click', () => {
    invitationText.textContent = '❤️ Tudo bem, mesmo assim você é muito especial para mim!';
    responseButtons.style.display = 'none';
  });
</script>
</body>
</html>
