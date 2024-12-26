<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Loja Elite de Pods</title>
    <style>
        /* Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            background: #f5f5f5;
            color: #333;
            overflow-x: hidden;
        }

        /* Cabeçalho */
        header {
            position: sticky;
            top: 0;
            background: linear-gradient(to right, #007BFF, #0056b3);
            padding: 1rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            z-index: 1000;
        }

        header .container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        header h1 {
            color: white;
            font-size: 2rem;
        }

        header nav ul {
            list-style: none;
            display: flex;
            gap: 1rem;
        }

        header nav ul li {
            position: relative;
        }

        header nav ul li a {
            color: white;
            text-decoration: none;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            transition: background 0.3s;
        }

        header nav ul li a:hover {
            background: rgba(255, 255, 255, 0.2);
        }

        /* Banner */
        .banner {
            height: 80vh;
            background: url('https://via.placeholder.com/1920x800') no-repeat center center/cover;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            position: relative;
            overflow: hidden;
        }

        .banner::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.4);
            z-index: 1;
        }

        .banner-content {
            position: relative;
            z-index: 2;
        }

        .banner h2 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .banner p {
            font-size: 1.5rem;
            margin-bottom: 2rem;
        }

        .banner a {
            display: inline-block;
            background: #007BFF;
            color: white;
            padding: 1rem 2rem;
            border-radius: 25px;
            text-decoration: none;
            font-size: 1.2rem;
            transition: background 0.3s;
        }

        .banner a:hover {
            background: #0056b3;
        }

        /* Produtos */
        #produtos {
            padding: 2rem 1rem;
        }

        #produtos h2 {
            text-align: center;
            font-size: 2rem;
            margin-bottom: 2rem;
        }

        .produtos-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .produto {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            position: relative;
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
            padding: 1.5rem;
            text-align: center;
        }

        .produto-content h3 {
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
        }

        .produto-content p {
            font-size: 1rem;
            margin-bottom: 1rem;
            color: #555;
        }

        .produto-content button {
            background: linear-gradient(to right, #007BFF, #0056b3);
            color: white;
            border: none;
            padding: 0.5rem 1.5rem;
            border-radius: 25px;
            cursor: pointer;
            font-size: 1rem;
            transition: background 0.3s;
        }

        .produto-content button:hover {
            background: linear-gradient(to right, #0056b3, #003f7f);
        }

        /* Sobre */
        #sobre {
            padding: 4rem 1rem;
            background: #f5f5f5;
            text-align: center;
        }

        #sobre h2 {
            font-size: 2rem;
            margin-bottom: 1rem;
        }

        #sobre p {
            max-width: 800px;
            margin: 0 auto;
            font-size: 1.2rem;
            line-height: 1.8;
        }

        /* Rodapé */
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 1rem;
            margin-top: 2rem;
        }

        footer p {
            font-size: 0.9rem;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Loja Elite de Pods</h1>
            <nav>
                <ul>
                    <li><a href="#produtos">Produtos</a></li>
                    <li><a href="#sobre">Sobre</a></li>
                    <li><a href="#contato">Contato</a></li>
                </ul>
            </nav>
        </div>
    </header>
    <div class="banner">
        <div class="banner-content">
            <h2>Encontre o Pod Perfeito</h2>
            <p>Os melhores preços e qualidade garantida!</p>
            <a href="#produtos">Ver Produtos</a>
        </div>
    </div>
    <main>
        <section id="produtos">
            <h2>Produtos em Destaque</h2>
            <div class="produtos-container">
                <div class="produto">
                    <img src="https://via.placeholder.com/300" alt="Pod Modelo 1">
                    <div class="produto-content">
                        <h3>Pod Modelo 1</h3>
                        <p>R$ 99,90</p>
                        <button>Comprar</button>
                    </div>
                </div>
                <div class="produto">
                    <img src="https://via.placeholder.com/300" alt="Pod Modelo 2">
                    <div class="produto-content">
                        <h3>Pod Modelo 2</h3>
                        <p>R$ 129,90</p>
                        <button>Comprar</button>
                    </div>
                </div>
                <div class="produto">
                    <img src="https://via.placeholder.com/300" alt="Pod Modelo 3">
                    <div class="produto-content">
                        <h3>Pod Modelo 3</h3>
                        <p>R$ 149,90</p>
                        <button>Comprar</button>
                    </div>
                </div>
            </div>
        </section>
        <section id="sobre">
            <h2>Sobre Nós</h2>
            <p>Na Loja Elite de Pods, nosso objetivo é proporcionar produtos de alta qualidade com os melhores preços do mercado. Inovação e satisfação garantida!</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Loja Elite de Pods. Todos os direitos reservados.</p>
    </footer>
</body>
</html>
