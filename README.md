<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Toyota Express</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <div class="logo">
            <img src="logo.png" alt="Toyota Express">
        </div>
        <nav>
            <ul>
                <li><a href="#inicio">Início</a></li>
                <li><a href="#veiculos">Veículos</a></li>
                <li><a href="#pecas">Peças</a></li>
                <li><a href="#contacto">Contato</a></li>
            </ul>
        </nav>
    </header>

    <section id="inicio" class="banner">
        <h1>Bem-vindo à Toyota Express</h1>
        <p>As melhores viaturas e peças com preços imbatíveis!</p>
    </section>

    <section id="veiculos">
        <h2>Veículos Disponíveis</h2>
        <div class="container">
            <div class="card">
                <img src="hilux.jpg" alt="Toyota Hilux">
                <h3>Toyota Hilux</h3>
                <p>Preço: <span class="preco">35.000.000 Kz</span></p>
            </div>
            <div class="card">
                <img src="prado.jpg" alt="Toyota Prado">
                <h3>Toyota Prado</h3>
                <p>Preço: <span class="preco">55.000.000 Kz</span></p>
            </div>
            <div class="card">
                <img src="corolla.jpg" alt="Toyota Corolla">
                <h3>Toyota Corolla</h3>
                <p>Preço: <span class="preco">20.000.000 Kz</span></p>
            </div>
        </div>
    </section>

    <section id="pecas">
        <h2>Peças Genuínas</h2>
        <div class="container">
            <div class="card">
                <img src="filtro.jpg" alt="Filtro de Óleo">
                <h3>Filtro de Óleo</h3>
                <p>Preço: <span class="preco">12.000 Kz</span></p>
            </div>
            <div class="card">
                <img src="pneu.jpg" alt="Pneu 16'">
                <h3>Pneu 16'</h3>
                <p>Preço: <span class="preco">45.000 Kz</span></p>
            </div>
            <div class="card">
                <img src="bateria.jpg" alt="Bateria 12V">
                <h3>Bateria 12V</h3>
                <p>Preço: <span class="preco">85.000 Kz</span></p>
            </div>
        </div>
    </section>

    <section id="contacto">
        <h2>Contato</h2>
        <p><strong>Telefone:</strong> +244 974 058 806</p>
        <p><strong>Email:</strong> muximaviagens21@gmail.com</p>
    </section>

    <footer>
        <p>&copy; 2025 Toyota Express - Todos os direitos reservados.</p>
    </footer>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background: #f4f4f4;
}

header {
    background: #c00;
    color: white;
    display: flex;
    justify-content: space-between;
    padding: 10px 20px;
    align-items: center;
}

.logo img {
    height: 50px;
}

nav ul {
    list-style: none;
    display: flex;
    gap: 20px;
}

nav ul li a {
    text-decoration: none;
    color: white;
    font-weight: bold;
}

.banner {
    background: url('carro-banner.jpg') no-repeat center center/cover;
    height: 300px;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    text-align: center;
}

.container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
    padding: 20px;
}

.card {
    background: white;
    padding: 15px;
    border-radius: 10px;
    width: 250px;
    text-align: center;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
}

.card img {
    width: 100%;
    border-radius: 10px;
}

.preco {
    color: #c00;
    font-weight: bold;
}

#contacto {
    background: #222;
    color: white;
    text-align: center;
    padding: 20px;
}

footer {
    background: #111;
    color: white;
    text-align: center;
    padding: 10px;
}
document.addEventListener("DOMContentLoaded", function() {
    let precos = document.querySelectorAll(".preco");
    precos.forEach(preco => {
        preco.style.fontSize = "1.2em";
        preco.style.transition = "0.5s";
        preco.addEventListener("mouseover", function() {
            preco.style.color = "gold";
            preco.style.fontSize = "1.4em";
        });
        preco.addEventListener("mouseout", function() {
            preco.style.color = "#c00";
            preco.style.fontSize = "1.2em";
        });
    });
});
</body>
</html>
