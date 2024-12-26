<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Loja 100% Funcional de Pods</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Roboto', sans-serif;
            color: #333;
            background: #f9f9f9;
        }

        header {
            background: linear-gradient(to right, #00c6ff, #0072ff);
            color: white;
            padding: 1rem;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 1.5rem;
        }

        nav ul li a {
            text-decoration: none;
            color: white;
            padding: 0.5rem 1rem;
            border-radius: 25px;
            transition: background 0.3s ease-in-out;
        }

        nav ul li a:hover {
            background: rgba(255, 255, 255, 0.2);
        }

        .banner {
            height: 70vh;
            background: url('https://via.placeholder.com/1920x800') no-repeat center center/cover;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            text-align: center;
            position: relative;
        }

        .banner::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.4);
        }

        .banner h2 {
            font-size: 3rem;
        }

        .products-section {
            padding: 4rem 1rem;
            background: #fff;
        }

        .products-section h2 {
            text-align: center;
            margin-bottom: 2rem;
            font-size: 2.5rem;
        }

        .product-card {
            background: white;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
            max-width: 300px;
        }

        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
        }

        .product-card img {
            width: 100%;
            height: 250px;
            object-fit: cover;
        }

        .product-card-content {
            padding: 1rem;
            text-align: center;
        }

        .product-card-content h3 {
            font-size: 1.8rem;
            margin-bottom: 0.5rem;
        }

        .product-card-content p {
            font-size: 1.2rem;
            color: #555;
            margin-bottom: 1rem;
        }

        .product-card-content button {
            background: #0072ff;
            color: white;
            border: none;
            padding: 0.8rem 1.5rem;
            border-radius: 25px;
            cursor: pointer;
            font-size: 1rem;
            transition: background 0.3s ease-in-out;
        }

        .product-card-content button:hover {
            background: #0056b3;
        }

        .cart {
            padding: 4rem 1rem;
            background: #f5f5f5;
            text-align: center;
        }

        .cart h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .cart-table {
            width: 80%;
            margin: 0 auto;
            border-collapse: collapse;
        }

        .cart-table th, .cart-table td {
            padding: 1rem;
            border: 1px solid #ddd;
        }

        .cart-table th {
            background-color: #0072ff;
            color: white;
        }

        .cart-table tr:hover {
            background-color: rgba(0, 114, 255, 0.1);
        }

        .cart-table img {
            width: 50px;
            height: auto;
        }

        .checkout-section {
            padding: 4rem 1rem;
            background: #fff;
            text-align: center;
        }

        .checkout-section form {
            max-width: 600px;
            margin: 0 auto;
        }

        .checkout-section input, 
        .checkout-section textarea {
            width: 100%;
            padding: 0.8rem;
            margin-bottom: 1rem;
            border: 1px solid #ddd;
            border-radius: 8px;
        }

        .checkout-section button {
            background: #0072ff;
            color: white;
            border: none;
            padding: 0.8rem 1.5rem;
            border-radius: 25px;
            cursor: pointer;
            font-size: 1rem;
            transition: background 0.3s ease-in-out;
        }

        .checkout-section button:hover {
            background: #0056b3;
        }

        footer {
            background: #333;
            color: white;
            padding: 1rem;
            text-align: center;
        }

        footer p {
            font-size: 0.9rem;
        }

        /* Responsividade */
        @media (max-width: 768px) {
            .banner h2 {
                font-size: 2.5rem;
            }

            .product-card img {
                height: 200px;
            }

            .product-card-content h3 {
                font-size: 1.6rem;
            }

            .product-card-content p {
                font-size: 1rem;
            }

            .cart-table {
                width: 100%;
            }
        }

    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Loja 100% Funcional de Pods</h1>
            <nav>
                <ul>
                    <li><a href="#produtos">Produtos</a></li>
                    <li><a href="#carrinho">Carrinho</a></li>
                    <li><a href="#checkout">Checkout</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <div class="banner">
        <div class="banner-content">
            <h2>Descubra o Melhor Pod do Mercado</h2>
            <p>Qualidade e inovação ao seu alcance!</p>
        </div>
    </div>

    <main>
        <section class="products-section" id="produtos">
            <h2>Produtos em Destaque</h2>
            <div class="products-container">
                <div class="product-card">
                    <img src="https://via.placeholder.com/300" alt="Pod Modelo 1">
                    <div class="product-card-content">
                        <h3>Pod Modelo 1</h3>
                        <p>R$ 99,90</p>
                        <button data-product="1">Adicionar ao Carrinho</button>
                    </div>
                </div>
                <div class="product-card">
                    <img src="https://via.placeholder.com/300" alt="Pod Modelo 2">
                    <div class="product-card-content">
                        <h3>Pod Modelo 2</h3>
                        <p>R$ 129,90</p>
                        <button data-product="2">Adicionar ao Carrinho</button>
                    </div>
                </div>
                <div class="product-card">
                    <img src="https://via.placeholder.com/300" alt="Pod Modelo 3">
                    <div class="product-card-content">
                        <h3>Pod Modelo 3</h3>
                        <p>R$ 149,90</p>
                        <button data-product="3">Adicionar ao Carrinho</button>
                    </div>
                </div>
            </div>
        </section>

        <section class="cart" id="carrinho">
            <h2>Carrinho de Compras</h2>
            <table class="cart-table">
                <thead>
                    <tr>
                        <th>Imagem</th>
                        <th>Produto</th>
                        <th>Preço</th>
                        <th>Quantidade</th>
                        <th>Ações</th>
                    </tr>
                </thead>
                <tbody id="cart-items">
                    <!-- Itens serão adicionados via JavaScript -->
                </tbody>
            </table>
        </section>

        <section class="checkout-section" id="checkout">
            <h2>Finalizar Compra</h2>
            <form id="checkout-form">
                <input type="text" placeholder="Nome" required>
                <input type="email" placeholder="Email" required>
                <textarea rows="5" placeholder="Endereço de Entrega"></textarea>
                <button type="submit">Finalizar Pedido</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Loja 100% Funcional de Pods. Todos os direitos reservados.</p>
    </footer>

    <script>
        let cart = [];

        document.querySelectorAll('button[data-product]').forEach(button => {
            button.addEventListener('click', () => {
                let productId = button.getAttribute('data-product');
                let productName = button.closest('.product-card-content').querySelector('h3').innerText;
                let productPrice = button.closest('.product-card-content').querySelector('p').innerText;

                // Adicionar ao carrinho
                cart.push({ id: productId, name: productName, price: productPrice });
                updateCart();
            });
        });

        function updateCart() {
            let cartItems = document.getElementById('cart-items');
            cart
