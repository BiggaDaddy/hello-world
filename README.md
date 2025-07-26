<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cigarette Store</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <!-- Age Verification Modal -->
    <div id="age-modal" class="modal">
        <div class="modal-content">
            <h2>Age Verification</h2>
            <p>You must be 21 or older to enter this site.</p>
            <button onclick="verifyAge(true)">I am 21+</button>
            <button onclick="verifyAge(false)">I am under 21</button>
        </div>
    </div>

    <!-- Health Warning -->
    <div class="health-warning">
        ⚠️ Smoking causes cancer and heart disease. This site is for adults 21+ only.
    </div>

    <!-- Header -->
    <header>
        <h1>Classic Cigarettes</h1>
        <nav>
            <a href="#">Home</a>
            <a href="#">Products</a>
            <a href="#">Terms</a>
            <a href="#">Contact</a>
        </nav>
    </header>

    <!-- Products -->
    <main class="product-grid">
        <div class="product-card">
            <img src="https://via.placeholder.com/200x150" alt="Product 1">
            <h3>Brand A - Classic</h3>
            <p>$8.99</p>
            <button>Add to Cart</button>
        </div>

        <div class="product-card">
            <img src="https://via.placeholder.com/200x150" alt="Product 2">
            <h3>Brand B - Menthol</h3>
            <p>$9.49</p>
            <button>Add to Cart</button>
        </div>

        <div class="product-card">
            <img src="https://via.placeholder.com/200x150" alt="Product 3">
            <h3>Brand C - Light</h3>
            <p>$8.49</p>
            <button>Add to Cart</button>
        </div>
    </main>

    <!-- Footer -->
    <footer>
        <p>© 2025 Classic Cigarettes Co. | This site is for legal adults only. Check your local laws before purchasing.</p>
    </footer>

    <script>
        function verifyAge(isOfAge) {
            const modal = document.getElementById('age-modal');
            if (isOfAge) {
                modal.style.display = 'none';
            } else {
                alert("You must be 21 or older to access this site.");
                window.location.href = "https://www.google.com";
            }
        }

        window.onload = function () {
            document.getElementById('age-modal').style.display = 'flex';
        }
    </script>
</body>
</html>
