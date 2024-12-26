<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lojinha de Pods</title>
    <style>
        body {
            font-family: 'Helvetica', 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f9fa;
        }
        header {
            background-color: #007bff;
            color: white;
            text-align: center;
            padding: 1rem 0;
        }
        nav {
            text-align: center;
            margin: 1rem 0;
        }
        nav a {
            margin: 0 1rem;
            text-decoration: none;
            color: #007bff;
            font-weight: bold;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background-color: white;
            padding: 2rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }
        .product {
            display: flex;
            align-items: center;
            border-bottom: 1px solid #e0e0e0;
            padding: 1rem 0;
        }
        .product img {
            width: 150px;
            height: 150px;
            margin-right: 2rem;
            border-radius: 8px;
        }
        .product-info {
            flex-grow: 1;
        }
        .product-info h3 {
            margin: 0;
            font-size: 1.5rem;
            color: #333;
        }
        .product-info p {
            margin: 0.5rem 0;
            color: #666;
        }
        .product-info .price {
            font-weight: bold;
            color: #007bff;
            font-size: 1.25rem;
        }
        .payment-options {
            text-align: center;
            margin: 2rem 0;
        }
        .payment-options img {
            width: 100px;
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
    <h2>Nossos Produtos</h2>

    <!-- Produto 1 -->
    <div class="product">
        <img src="https://via.placeholder.com/150" alt="Pod">
        <div class="product-info">
            <h3>Pod Recarregável Premium</h3>
            <p>Delicioso sabor de mentol fresco</p>
            <p class="price">R$ 39,90</p>
        </div>
    </div>

    <!-- Produto 2 -->
    <div class="product">
        <img src="https://via.placeholder.com/150" alt="Pod">
        <div class="product-info">
            <h3>Pod Frutado</h3>
            <p>Sabor de frutas cítricas refrescantes</p>
            <p class="price">R$ 34,90</p>
        </div>
    </div>

    <!-- Adicione mais produtos conforme necessário -->

    <div class="payment-options">
        <h3>Formas de Pagamento</h3>
        <img src="https://via.placeholder.com/100x50" alt="Pix">
        <img src="https://via.placeholder.com/100x50" alt="Cartão de Crédito">
        <img src="https://via.placeholder.com/100x50" alt="Boleto Bancário">
    </div>
</div>

</body>
</html>
