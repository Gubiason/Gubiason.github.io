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

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #333;
    color: white;
    padding: 1rem;
    text-align: center;
}

header nav ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: center;
}

header nav ul li {
    margin: 0 1rem;
}

header nav ul li a {
    color: white;
    text-decoration: none;
}

main {
    padding: 2rem;
}

.produto {
    border: 1px solid #ccc;
    padding: 1rem;
    margin: 1rem;
    text-align: center;
}

.produto img {
    max-width: 100%;
    height: auto;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 1rem;
    position: fixed;
    bottom: 0;
    width: 100%;
}
