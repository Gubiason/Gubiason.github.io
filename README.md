<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Loja Premium de Pods</title>
    <style>
        /* Reset básico */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            background: linear-gradient(to bottom, #f9f9f9, #eaeaea);
            color: #333;
        }

        /* Cabeçalho */
        header {
            background: linear-gradient(to right, #007BFF, #0056b3);
            color: white;
            padding: 1rem 0;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        header h1 {
            font-size: 2.5rem;
            font-weight: bold;
            margin-bottom: 0.5rem;
        }

        header nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            gap: 1.5rem;
        }

        header nav ul li a {
            color: white;
            text-decoration: none;
            padding: 0.5rem 1rem;
            border: 2px solid transparent;
            border-radius: 25px;
            transition: all 0.3s;
        }

        header nav ul li a:hover {
            background: white;
            color: #0056b3;
            border: 2px solid #0056b3;
        }

        /* Banner */
        .banner {
            background: url('https://via.placeholder.com/1920x400') no-repeat center/cover;
            color: white;
            text-align: center;
            padding: 4rem 1rem;
        }

        .banner h2 {
            font-size: 2rem;
            margin-bottom: 1rem;
        }

        .banner p {
            font-size: 1.2rem;
        }

        /* Produtos */
        #produtos {
            padding: 2rem 1rem;
            background: #fff;
        }

        #produtos h2 {
            text-align: center;
            margin-bottom: 2rem;
            font-size: 2rem;
        }

        .produtos-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .produto {
            background: #f9f9f9;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .produto:hover {
            transform: translateY(-10px);
            box-shadow: 0 6px 10px rgba(0, 0, 0, 0.15);
        }

        .produto img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .produto-content {
            padding: 1rem;
            text-align: center;
        }

        .produto-content h3 {
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
        }

        .produto-content p {
            font-size: 1rem;
            margin-bottom: 1rem;
            color: #555;
        }

        .produto-content button {
            background: #007BFF;
            color: white;
            border: none;
            padding: 0.5rem 1.5rem;
            border-radius: 25px;
            cursor: pointer;
            transition: background 0.3s;
        }

        .produto-content button:hover {
            background: #0056b3;
        }

        /* Sobre */
        #sobre {
            padding: 2rem 1rem;
            background: #eaeaea;
            text-align: center;
        }

        #sobre h2 {
            margin-bottom: 1rem;
        }

        #sobre p {
            max-width: 800px;
            margin: 0 auto;
            line-height: 1.8;
        }

        /* Contato */
        #contato {
            padding: 2rem 1rem;
            background: #fff;
        }

        #contato form {
            max-width: 600px;
            margin: 0 auto;
            background: white;
            padding: 1rem;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        #contato form label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: bold;
        }

        #contato form input, #contato form textarea, #contato form button {
            width: 100%;
            margin-bottom: 1rem;
            padding: 0.8rem;
            border: 1px solid #ddd;
            border-radius: 5px;
        }

        #contato form button {
            background: #007BFF;
            color: white;
            border: none;
            cursor: pointer;
            transition: background 0.3s;
        }

        #contato form button:hover {
            background: #0056b3;
        }

        /* Rodapé */
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 1rem;
        }

        footer p {
            font-size: 0.9rem;
        }
    </style>
</head>
<body>
    <header>
        <h1>Loja Premium de Pods</h1>
        <nav>
            <ul>
                <li><a href="#produtos">Produtos</a></li>
                <li><a href="#sobre">Sobre</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
    </header>
    <div class="banner">
        <h2>Encontre o Pod Perfeito</h2>
        <p>Os melhores preços e qualidade garantida!</p>
    </div>
    <main>
        <section id="produtos">
            <h2>Produtos em Destaque</h2>
            <div class="produtos-container">
                <div class="produto">
                    <img src="https://via.placeholder.com/300" alt="Pod Modelo 1">
                    <div class="produto-content">
                        <h3>Pod Modelo 1</h3>
                        <p>Preço: R$ 99,90</p>
                        <button>Comprar</button>
                    </div>
                </div>
                <div class="produto">
                    <img src="https://via.placeholder.com/300" alt="Pod Modelo 2">
                    <div class="produto-content">
                        <h3>Pod Modelo 2</h3>
                        <p>Preço: R$ 129,90</p>
                        <button>Comprar</button>
                    </div>
                </div>
                <div class="produto">
                    <img src="https://via.placeholder.com/300" alt="Pod Modelo 3">
                    <div class="produto-content">
                        <h3>Pod Modelo 3</h3>
                        <p>Preço: R$ 149,90</p>
                        <button>Comprar</button>
                    </div>
                </div>
            </div>
        </section>
        <section id="sobre">
            <h2>Sobre Nós</h2>
            <p>Na Loja Premium de Pods, nosso compromisso é oferecer os melhores produtos do mercado. Qualidade, confiança e inovação são os nossos pilares.</p>
        </section>
        <section id="contato">
            <h2>Contato</h2>
            <form>
                <label for="nome">Nome:</label>
                <input type="text" id="nome" name="nome" placeholder="Digite seu nome" required>
                <label for="email">E-mail:</label>
                <input type="email" id="email" name="email" placeholder="Digite seu e-mail" required>
                <label for="mensagem">Mensagem:</label>
                <textarea id="mensagem" name="mensagem" rows="5" placeholder="Digite sua mensagem" required></textarea>
                <button type="submit">Enviar</button>
            </form>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Loja Premium de Pods. Todos os direitos reservados.</p>
    </footer>
</body>
</html>
