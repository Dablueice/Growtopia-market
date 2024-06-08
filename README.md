<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Growtopia Market</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
        }
        h1 {
            text-align: center;
        }
        .container {
            width: 80%;
            margin: auto;
        }
        .item {
            border: 1px solid #ccc;
            padding: 10px;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <h1>Growtopia Market</h1>
    <div class="container">
        <div class="item">
            <h2>Account</h2>
            <p>Price: Rp 100.000</p>
            <button onclick="buyItem('account')">Buy Now</button>
        </div>
        <div class="item">
            <h2>Diamond Lock</h2>
            <p>Price: Rp 4.500 per DL</p>
            <button onclick="buyItem('diamondlock')">Buy Now</button>
        </div>
    </div>

    <script>
        function buyItem(item) {
            if (item === 'account') {
                alert('You have purchased an account for Rp 100.000');
            } else if (item === 'diamondlock') {
                var quantity = prompt('How many Diamond Locks do you want to buy?');
                if (quantity !== null && !isNaN(quantity) && quantity > 0) {
                    var totalPrice = quantity * 4500;
                    alert('You have purchased ' + quantity + ' Diamond Lock(s) for Rp ' + totalPrice);
                } else {
                    alert('Invalid quantity');
                }
            }
        }
    </script>
</body>
</html>
