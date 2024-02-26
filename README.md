<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Atlas FC</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #1E1E1E; /* Preto */
            color: #FFD700; /* Amarelo escuro */
            scroll-behavior: smooth; /* Adiciona rolagem suave */
        }

        header {
            background-color: #000;
            color: #FFD700;
            text-align: center;
            padding: 10px;
        }

        nav {
            background-color: #333;
            color: #FFD700;
            text-align: center;
            padding: 10px;
        }

        nav a {
            color: #FFD700;
            text-decoration: none;
            padding: 10px;
            margin: 0 5px;
            cursor: pointer;
        }

        section {
            padding: 20px;
        }

        footer {
            background-color: #000;
            color: #FFD700;
            text-align: center;
            padding: 10px;
            position: absolute;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>Atlas Futebol Clube</h1>
    </header>

    <nav>
        <a class="nav-link" href="#home">Home</a>
        <a class="nav-link" href="#sobre">Sobre</a>
        <a class="nav-link" href="calendario.html">Calendário</a>
        <a class="nav-link" href="#contato">Contato</a>
    </nav>

    <section id="home">
        <h2>Bem-vindo ao site oficial do Atlas FC!</h2>
        <p>Confira as últimas notícias, resultados e informações sobre o nosso time.</p>
    </section>

    <section id="sobre">
        <h2>Sobre o Atlas FC</h2>
        <p>Conheça a história, conquistas e o elenco atual do Atlas Futebol Clube.</p>
    </section>

    <section id="contato">
        <h2>Entre em Contato</h2>
        <p>Envie-nos suas perguntas, sugestões ou comentários.</p>
    </section>

    <footer>
        <p>&copy; 2024 Atlas Futebol Clube. Todos os direitos reservados.</p>
    </footer>

    <script>
        document.querySelectorAll('.nav-link').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();

                if (this.getAttribute('href') === 'calendario.html') {
                    // Se clicar em "Calendário", redireciona para a página de calendário
                    window.location.href = 'calendario.html';
                } else {
                    // Para outras abas, rola suavemente para a seção correspondente
                    document.querySelector(this.getAttribute('href')).scrollIntoView({
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>
