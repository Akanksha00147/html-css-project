# html-css-project
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Online Store</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <style>
        * {
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background-color: #4CAF50;
            color: white;
            text-align: center;
            padding: 20px 0;
        }

        nav {
            text-align: center;
            margin: 20px 0;
        }

        nav button {
            margin: 0 10px;
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        nav button:hover {
            background-color: #45a049;
        }

        main {
            display: flex;
            justify-content: space-between;
            padding: 20px;
        }

        #products {
            display: flex;
            flex-wrap: wrap;
            width: 70%;
        }

        .product {
            background-color: white;
            border: 1px solid #ccc;
            border-radius: 5px;
            margin: 10px;
            padding: 10px;
            width: 200px;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .product:hover {
            transform: translateY(-5px);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .product img {
            width: 100%;
            border-radius: 5px;
        }

        .price {
            font-weight: bold;
            color: #4CAF50;
        }

        #cart {
            width: 25%;
            border-left: 1px solid #ccc;
            padding-left: 20px;
        }

        #cart h2 {
            margin-top: 0;
        }

        #cart-items {
            margin-bottom: 20px;
        }

        .checkout {
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .checkout:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to Our eCommerce Store</h1>
    </header>

    <nav id="categories">
        <button onclick="filterProducts('all')">All</button>
        <button onclick="filterProducts('electronics')">Electronics</button>
        <button onclick="filterProducts('clothing')">Clothing</button>
        <button onclick="filterProducts('home')">Home</button>
        <button onclick="filterProducts('books')">Books</button>
    </nav>

    <main>
        <div id="products">
            <!-- Sample Product 1 -->
            <div class="product" data-category="electronics">
                <img src="https://via.placeholder.com/150" alt="Product 1">
                <h3>Product 1</h3>
                <p>Description of Product 1</p>
                <p class="price">$100</p>
                <button class="add-to-cart" onclick="addToCart('Product 1')">Add to Cart <i class="fas fa-shopping-cart"></i></button>
            </div>

            <!-- Sample Product 2 -->
            <div class="product" data-category="clothing">
                <img src="https://via.placeholder.com/150" alt="Product 2">
                <h3>Product 2</h3>
                <p>Description of Product 2</p>
                <p class="price">$50</p>
                <button class="add-to-cart" onclick="addToCart('Product 2')">Add to Cart <i class="fas fa-shopping-cart"></i></button>
            </div
