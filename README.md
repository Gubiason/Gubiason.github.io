<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lojinha de Pods</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
        }
        header {
            background-color: #4CAF50;
            color: white;
            text-align: center;
            padding: 1rem;
        }
        nav {
            text-align: center;
            margin: 1rem 0;
        }
        nav a {
            margin: 0 1rem;
            text-decoration: none;
            color: #4CAF50;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            background-color: white;
            padding: 2rem;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        .product {
            display: flex;
            align-items: center;
            margin-bottom: 1rem;
        }
        .product img {
            width: 100px;
            height: 100px;
            margin-right: 1rem;
        }
        .product-info {
            flex-grow: 1;
        }
        .product-info h3 {
            margin: 0;
        }
        .product-info p {
            margin: 0.5rem 0;
            color: #555;
        }
        .product-info .price {
            font-weight: bold;
            color: #4CAF50;
        }
        .payment-options {
            text-align: center;
            margin: 2rem 0;
        }
        .payment-options img {
            width: 80px;
            margin: 0 1rem;
        }
    </style>
</head>
<body>

<header>
    <h1>Lojinha de Pods</h1>
</header>

<nav>
    <a href="#">Home</a>
    <a href="#">Produtos</a>
    <a href="#">Contato</a>
</nav>

<div class="container">
    <h2>Produtos</h2>

    <div class="product">
        <img src="https://via.placeholder.com/100" alt="Pod">
        <div class="product-info">
            <h3>Pod Recarregável</h3>
            <p>Delicioso sabor de frutas tropicais</p>
            <p class="price">R$ 29,90</p>
        </div>
    </div>

    <!-- Adicione mais produtos aqui -->

    <div class="payment-options">
        <h3>Formas de Pagamento</h3>
        <img src="https://via.placeholder.com/80x40" alt="Pix">
        <img src="https://via.placeholder.com/80x40" alt="Cartão de Crédito">
        <img src="https://via.placeholder.com/80x40" alt="Boleto Bancário">
    </div>
</div>

</body>
</html>

