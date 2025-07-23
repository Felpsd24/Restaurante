# Restaurante
Como faço para deixa-lo mais imersivo? Por exemplo: Clico em um certo prato e aparece a foto.
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Restaurante FLP</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #fff8f0;
      color: #333;
    }

    header {
      background-color: #a83232;
      color: white;
      padding: 20px 0;
      text-align: center;
    }

    nav {
      background-color: #6e1e1e;
      text-align: center;
      padding: 10px 0;
    }

    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }

    .container {
      color:#6e1e1e;
      padding: 40px 20px;
      max-width: 1000px;
      margin: auto;
    }

    .menu {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .card {
      background-color: #fff;
      border: 1px solid #ddd;
      border-radius: 8px;
      padding: 20px;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 20px 10px;
      margin-top: 40px;
    }

    h1, h2 {
      color: #a83232;
    }

    .horarios, .contato {
      margin-top: 40px;
    }
  </style>
</head>
<body>

  <header>
    <title>Restaurante FLP</title>
    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTV_Ts3ol3HRacV1TyPnz2eq4B6p0Pau5KrlA&s" style="width: 100px; height: auto;" alt="Chef wearing a white hat and red scarf smiling warmly in a kitchen setting with soft lighting, conveying a welcoming and friendly atmosphere. No visible text." >
    <h1>Restaurante do FLP</h1>
    <p>Sabores que conquistam</p>
  </header>

  <nav>
    <a href="#menu">Cardápio</a>
    <a href="#horarios">Horários</a>
    <a href="#contato">Contato</a>
  </nav>

  <div class="container">
    <section id="menu">
      <h2>Cardápio</h2>
      <div class="menu">
        <div class="card">
          <h3>Feijoada Completa</h3>
          <p>Feijão preto, carnes selecionadas, arroz e farofa.</p>
          <strong>R$ 32,00</strong>
          <style>
            .card h3 {
              color: #a83232;
            }
            .card p {
              color: #e9c916;
            }
          </style>
        </div>
        <div class="card">
          <h3>Prato Executivo</h3>
          <p>Arroz, feijão, bife acebolado, batata frita e salada.</p>
          <strong>R$ 25,00</strong>
        </div>
        <div class="card">
          <h3>Lasanha de Frango</h3>
          <p>Lasanha artesanal com molho branco e queijo gratinado.</p>
  <strong>R$ 28,00</strong>
</div>
        <div class="card">
          <h3>Suco Natural</h3>
          <p>Sabores variados: laranja, abacaxi, limão, acerola.</p>
          <strong>R$ 6,00</strong>
        </div>
      </div>
    </section>

    <section class="horarios" id="horarios">
      <h2>Horários de Funcionamento</h2>
      <p>Segunda a Sexta: 10h às 15h</p>
      <p>Sábado e Domingo: 10h às 16h</p>
    </section>

    <section class="contato" id="contato">
      <h2>Contato</h2>
      <p>📍 Rua das Comidas, 000</p>
      <p>Telefone: (00) 00000-0000</p>
      <p>Email: restauranteflp@gmail.com</p>
    </section>
  </div>

  <footer>
    <p>Restaurante do FLP. Todos os direitos reservados.</p>
    <p class="creditos">Desenvolvido por Luiz Felipe</p>
  </footer>
  <script>
    document.querySelectorAll('nav a').forEach(link => {
      link.addEventListener('click', function(event) {
        event.preventDefault();
        const targetId = this.getAttribute('href').substring(1);
        const targetSection = document.getElementById(targetId);
        if (targetSection) {
          targetSection.scrollIntoView({ behavior: 'smooth' });
        }
      });
    });
  </script>
  <style>
    .creditos {
      margin: 0;
      padding: 5px 0;
    }
    #minhaCaixa.ativa {
      background: orange;
    }
  </style>
</body>
</html>
