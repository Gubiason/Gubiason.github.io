<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VIPpods</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>VIPpods</h1>
        <nav>
            <ul>
                <li><a href="#produtos">Produtos</a></li>
                <li><a href="#sobre">Sobre Nós</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="produtos">
            <h2>Nossos Produtos</h2>
            <div class="produto">
                <img src="pod1.jpg" alt="Pod Modelo 1">
                <h3>Pod Modelo 1</h3>
                <p>Descrição do produto.</p>
                <button>Comprar</button>
            </div>
            <div class="produto">
                <img src="pod2.jpg" alt="Pod Modelo 2">
                <h3>Pod Modelo 2</h3>
                <p>Descrição do produto.</p>
                <button>Comprar</button>
            </div>
        </section>
        <section id="sobre">
            <h2>Sobre Nós</h2>
            <p>Bem-vindo à nossa loja de pods! Oferecemos os melhores produtos do mercado.</p>
        </section>
        <section id="contato">
            <h2>Contato</h2>
            <form>
                <label for="nome">Nome:</label>
                <input type="text" id="nome" name="nome" required>
                <label for="email">E-mail:</label>
                <input type="email" id="email" name="email" required>
                <label for="mensagem">Mensagem:</label>
                <textarea id="mensagem" name="mensagem" required></textarea>
                <button type="submit">Enviar</button>
            </form>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Loja de Pods</p>
    </footer>
</body>
</html>
