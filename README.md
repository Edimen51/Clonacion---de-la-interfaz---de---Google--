# Clonacion---de-la-interfaz---de---Google--
Google - clonacion
Proyecto Interfaz Google
A continuación, se presenta el código para construir la interfaz estática de Google, cumpliendo con los requisitos de HTML semántico, CSS y estructura solicitada:
1. Estructura HTML (index.html)
html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Google</title>
    <link rel="stylesheet" href="styles.css">
    <!-- Íconos de Font Awesome (simula iconos de Google) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- HEADER: Sección superior con enlaces, iconos y perfil -->
    <header class="header">
        <nav class="header__nav">
            <ul class="header__links-left">
                <li><a href="#">Gmail</a></li>
                <li><a href="#">Imágenes</a></li>
            </ul>
            <ul class="header__links-right">
                <li><a href="#"><i class="fas fa-th"></i></a></li>
                <li><a href="#"><i class="fas fa-user-circle"></i></a></li>
            </ul>
        </nav>
    </header>

    <!-- MAIN: Contenido central -->
    <main class="main">
        <div class="main__logo">
            <img src="https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png" alt="Logo Google">
        </div>
        <div class="main__search">
            <input type="text" placeholder="Buscar con Google">
            <div class="main__search-icons">
                <i class="fas fa-search"></i>
                <i class="fas fa-microphone"></i>
            </div>
        </div>
        <div class="main__buttons">
            <button>Buscar con Google</button>
            <button>Voy a tener suerte</button>
        </div>
    </main>

    <!-- FOOTER: Enlaces inferiores -->
    <footer class="footer">
        <div class="footer__top">
            <p>México</p>
        </div>
        <div class="footer__bottom">
            <ul class="footer__links-left">
                <li><a href="#">Sobre Google</a></li>
                <li><a href="#">Publicidad</a></li>
                <li><a href="#">Negocios</a></li>
                <li><a href="#">Cómo funciona la búsqueda</a></li>
            </ul>
            <ul class="footer__links-right">
                <li><a href="#">Privacidad</a></li>
                <li><a href="#">Condiciones</a></li>
                <li><a href="#">Preferencias</a></li>
            </ul>
        </div>
    </footer>
</body>
</html>

2. Estilos CSS (styles.css)
css

/* Reset básico */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    font-size: 14px;
    line-height: 1.5;
}

/* HEADER */
.header {
    padding: 15px 20px;
}

.header__nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.header__links-left, .header__links-right {
    list-style: none;
    display: flex;
    gap: 15px;
}

.header__links-left a, .header__links-right a {
    text-decoration: none;
    color: #000;
    opacity: 0.8;
}

.header__links-right a {
    font-size: 18px;
}

.header__links-left a:hover, .header__links-right a:hover {
    text-decoration: underline;
}

/* MAIN */
.main {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: calc(100vh - 150px);
    gap: 25px;
}

.main__logo img {
    width: 272px;
    height: 92px;
}

.main__search {
    position: relative;
    width: 580px;
    max-width: 90%;
}

.main__search input {
    width: 100%;
    padding: 12px 45px;
    border: 1px solid #dfe1e5;
    border-radius: 24px;
    font-size: 16px;
}

.main__search input:hover, .main__search input:focus {
    box-shadow: 0 1px 6px rgba(32,33,36,.28);
    outline: none;
}

.main__search-icons {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    width: 100%;
    display: flex;
    justify-content: space-between;
    padding: 0 15px;
    color: #9aa0a6;
}

.main__buttons {
    display: flex;
    gap: 15px;
}

.main__buttons button {
    padding: 10px 16px;
    border: none;
    border-radius: 4px;
    background-color: #f8f9fa;
    color: #3c4043;
    cursor: pointer;
}

.main__buttons button:hover {
    border: 1px solid #dadce0;
    box-shadow: 0 1px 1px rgba(0,0,0,.1);
}

/* FOOTER */
.footer {
    background-color: #f2f2f2;
    color: #70757a;
}

.footer__top {
    padding: 15px 30px;
    border-bottom: 1px solid #dadce0;
}

.footer__bottom {
    display: flex;
    justify-content: space-between;
    padding: 15px 30px;
    flex-wrap: wrap;
}

.footer__links-left, .footer__links-right {
    list-style: none;
    display: flex;
    gap: 20px;
}

.footer__links-left a, .footer__links-right a {
    text-decoration: none;
    color: #70757a;
}

.footer__links-left a:hover, .footer__links-right a:hover {
    text-decoration: underline;
}

/* Adaptabilidad básica */
@media (max-width: 600px) {
    .footer__bottom {
        justify-content: center;
        gap: 15px;
    }
}

La interfaz replica la estructura y estilo básico de Google, utiliza HTML semántico, diferentes selectores CSS y cumple con los requisitos de control de versiones.
