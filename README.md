

---

# ⭐ Semana 5/6 — Taller de Ingenieria web

### Página estilo Steam: HTML + CSS con comentarios

## **1. Descripción General del Proyecto**

Durante esta semana se trabajó en la creación de una página web inspirada en la interfaz de **Steam**, la plataforma de videojuegos más popular
El objetivo del taller fue:

* Aplicar **Bootstrap 5** para crear componentes dinámicos
* Usar un **carousel** para destacar juegos importantes
* Crear tarjetas cards para mostrar juegos populares
* Aplicar estilos personalizados en un archivo CSS propio
* Integrar imágenes, botones y navegación responsive

La página final contiene:

* Un encabezado con menú
* Un carrusel dinámico
* Una sección de juegos destacados
* Un diseño visual similar al de Steam, usando colores oscuros y tarjetas estilizadas

---

## **2. Estructura del Proyecto**

El proyecto contiene:

* **index.html** → archivo principal con el contenido y estructura
* **estilos.css** → archivo para sobreescribir estilos de Bootstrap y agregar diseño propio

---

## **index.html**

```html
<!doctype html>
<html lang="es">
<head>
    <meta charset="utf-8">
    <title>STIM - Tienda de Juegos</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!--BootstrapCSS -->
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
      rel="stylesheet"
    > <!-- aqui estoy usando boostrap para tener los estilos base como grid, botones, textos y que todo se adapte -->

    <!-- CSS organizado -->
    <link rel="stylesheet" href="estilos/estilos.css"> <!-- mi css donde pongo mis colores y estilos propios -->
</head>

<body>
    <!-- TOP BAR estilo Steam -->
    <div class="top-bar"> <!-- barra arriba tipo steam -->
        <div class="container d-flex justify-content-between align-items-center"> <!-- aqui uso bootstrap pa alinear todo en una fila centrada -->
            <div>
                <span class="me-3">STIM</span>
                <a href="#">tienda</a> |
                <a href="#">comunidad</a> |
                <a href="#">acerca de</a>
            </div>
            <div>
    
                <a href="#" class="me-3">instalar stim</a>
            <a href="#" class="me-2">iniciar sesion</a>
            <span>$cero dolare USD</span>
            </div>
        </div>
    </div>
    <!-- NAVBAR principal -->
    <nav class="navbar navbar-expand-lg navbar-dark main-nav"> <!-- navbar de bootstrap para que sea responsive -->
        <div class="container">
            <a class="navbar-brand" href="#">STIM</a>

            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#mainMenu"> <!-- boton hamburguesa de boostrap -->
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="mainMenu"> <!-- menu que se abre y cierra -->
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item"><a class="nav-link active" href="#">TIENDA</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">COMUNIDAD</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">CHAT</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">SOPORTE</a></li>
                </ul>

                <form class="d-flex" role="search"> <!-- d-flex de bootstrap pa poner input y boton juntitos -->
                    <input class="form-control form-control-sm me-2" type="search" placeholder="buscar en la tienda"> <!-- input de busqueda -->
                    <button class="btn btn-sm btn-outline-info" type="submit">buscar</button> <!-- boton estilo boostrap -->
                </form>
            </div>
        </div>
    </nav>

    <!-- CONTENIDO GENERAL -->
    <div class="content-wrap">
        <div class="container py-4">

            <!-- BANNER Principal tipo Steam -->
            <div class="section-block hero-banner mb-4">
                <img src="https://cdn.akamai.steamstatic.com/steam/apps/1938090/library_hero.jpg"> <!-- imagen grande tipo portada -->
                <div class="hero-info"> <!-- info del banner -->
                    <span class="hero-tag">ya disponible</span>
                    <h1>CALL OF DUTY BLACK OPS</h1>
                    <p class="mb-2">Vive una nueva campaña, modos multijugador y experiencia zombies.</p>
                    <button class="hero-btn">ver en stim</button>
                </div>
            </div>

            <!-- DESTACADOS -->
            <div class="section-block">
                <div class="d-flex justify-content-between align-items-center mb-2"> <!-- uso bootstrap pa alinear -->
                    <h2 class="section-title mb-0">destacados y recomendados</h2>
                </div>

                <div id="carouselDestacados" class="carousel slide" data-bs-ride="carousel"> <!-- esto es un carrusel de bootstrap -->
                    <div class="carousel-inner">

                        <!-- SLIDE 1 -->
                        <div class="carousel-item active"> <!-- slide activo -->
                            <div class="row g-3"> <!-- fila de bootstrap con espacio -->

                                <div class="col-md-3"> <!-- col de tamaño 3 -->
                                    <div class="game-card"> <!-- tarjeta de juego mia -->
                                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/1091500/header.jpg"> <!-- imagen del juego -->
                                        <div class="game-body"> <!-- cuerpo de texto -->
                                            <p class="game-title">Cyberpunk 2077</p>
                                            <span class="discount">-50%</span> <!-- descuento -->
                                            <span class="old-price">$59.99</span> <!-- precio antiguo -->
                                            <span class="price-tag">$29.99</span> <!-- precio final -->
                                        </div>
                                    </div>
                                </div>

                                <div class="col-md-3">
                                    <div class="game-card">
                                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/1086940/header.jpg"> <!-- imagen del juego -->
                                        <div class="game-body">
                                            <p class="game-title">Baldur's Gate 3</p>
                                            <span class="price-tag">$59.99</span> <!-- este no tiene descuento -->
                                        </div>
                                    </div>
                                </div>

                                <div class="col-md-3">
                                    <div class="game-card">
                                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/271590/header.jpg">
                                        <div class="game-body">
                                            <p class="game-title">GTA V</p>
                                            <span class="discount">-63%</span>
                                            <span class="old-price">$29.99</span> <!-- precio viejo -->
                                            <span class="price-tag">$10.99</span> <!-- precio nuevo -->
                                        </div>
                                    </div>
                                </div>

                                <div class="col-md-3">
                                    <div class="game-card">
                                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/739630/header.jpg">
                                        <div class="game-body">
                                            <p class="game-title">Phasmophobia</p>
                                            <span class="price-tag">$13.99</span>
                                        </div>
                                    </div>
                                </div>

                            </div>
                        </div>

                        <!-- SLIDE 2 -->
                        <div class="carousel-item">
                            <div class="row g-3">

                                <div class="col-md-3">
                                    <div class="game-card">
                                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/892970/header.jpg"> <!-- imagen -->
                                        <div class="game-body">
                                            <p class="game-title">Valheim</p>
                                            <span class="price-tag">$19.99</span>
                                        </div>
                                    </div>
                                </div>

                                <div class="col-md-3">
                                    <div class="game-card">
                                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/1245620/header.jpg">
                                        <div class="game-body">
                                            <p class="game-title">Elden Ring</p>
                                            <span class="price-tag">$59.99</span>
                                        </div>
                                    </div>
                                </div>

                                <div class="col-md-3">
                                    <div class="game-card">
                                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/1238810/header.jpg"> <!-- header del juego -->
                                        <div class="game-body">
                                            <p class="game-title">EA Sports FC</p>
                                            <span class="discount">-40%</span>
                                            <span class="old-price">$69.99</span> <!-- precio anterior -->
                                            <span class="price-tag">$41.99</span> <!-- precio actual -->
                                        </div>
                                    </div>
                                </div>

                                <div class="col-md-3">
                                    <div class="game-card">
                                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/1174180/header.jpg">
                                        <div class="game-body">
                                            <p class="game-title">Red Dead Redemption 2</p>
                                            <span class="discount">-67%</span>
                                            <span class="old-price">$59.99</span> <!-- precio antes -->
                                            <span class="price-tag">$19.79</span> <!-- nuevo precio -->
                                        </div>
                                    </div>
                                </div>

                            </div>
                        </div>

                    </div>

                    <button class="carousel-control-prev" type="button" data-bs-target="#carouselDestacados" data-bs-slide="prev"> <!-- boton pa mover el carrusel -->
                        <span class="carousel-control-prev-icon"></span> <!-- icono izquierdo -->
                    </button>
                    <button class="carousel-control-next" type="button" data-bs-target="#carouselDestacados" data-bs-slide="next"> <!-- boton derecha -->
                        <span class="carousel-control-next-icon"></span>
                    </button>
                </div>
            </div>

            <!-- DESCUENTOS Y EVENTOS -->
            <div class="section-block">
                <div class="d-flex justify-content-between align-items-center mb-2"> <!-- uso bootstrap para alinear -->
                    <h2 class="section-title mb-0">descuentos y eventos</h2>
                    <a href="#" class="btn btn-sm btn-outline-info">ver más</a>
                </div>

                <div class="row g-3">
                    <div class="col-md-4">
                        <div class="game-card">
                            <img src="https://cdn.akamai.steamstatic.com/steam/apps/1145360/header.jpg"> <!-- img del juego -->
                            <div class="game-body">
                                <p class="game-title">Hades II</p>
                                <span class="discount">-20%</span>
                                <span class="old-price">$14.99</span> <!-- precio viejo -->
                                <span class="price-tag">$11.99</span>
                            </div>
                        </div>
                    </div>

                    <div class="col-md-4">
                        <div class="game-card">
                            <img src="https://cdn.akamai.steamstatic.com/steam/apps/1874880/header.jpg"> <!-- header del juego -->
                            <div class="game-body">
                                <p class="game-title">Arma Reforger</p>
                                <span class="discount">-30%</span>
                                <span class="old-price">$24.99</span> <!-- este es el precio antiguo -->
                                <span class="price-tag">$17.49</span> <!-- precio pagable ahora -->
                            </div>
                        </div>
                    </div>

                    <div class="col-md-4">
                        <div class="game-card">
                            <img src="https://cdn.akamai.steamstatic.com/steam/apps/1291340/header.jpg">
                            <div class="game-body">
                                <p class="game-title">Mini Motorways</p>
                                <span class="discount">-25%</span>
                                <span class="old-price">$5.79</span> <!-- el precio original -->
                                <span class="price-tag">$4.34</span> <!-- precio con descuento -->
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- CATEGORÍAS -->
            <div class="section-block">
                <h2 class="section-title">explorar por categoría</h2>

                <div class="row g-3">

                    <div class="col-md-3">
                        <div class="category-card">
                            <img src="https://cdn.akamai.steamstatic.com/steam/apps/739630/header.jpg"> <!-- imagen -->
                            <div class="category-name">terror</div> <!-- categoria -->
                        </div>
                    </div>

                    <div class="col-md-3">
                        <div class="category-card">
                            <img src="https://cdn.akamai.steamstatic.com/steam/apps/601150/header.jpg">
                            <div class="category-name">novelas visuales</div>
                        </div>
                    </div>

                    <div class="col-md-3">
                        <div class="category-card">
                            <img src="https://cdn.akamai.steamstatic.com/steam/apps/1238810/header.jpg">
                            <div class="category-name">deportes</div>
                        </div>
                    </div>

                    <div class="col-md-3">
                        <div class="category-card">
                            <img src="https://cdn.akamai.steamstatic.com/steam/apps/892970/header.jpg">
                            <div class="category-name">cooperativos</div>
                        </div>
                    </div>

                </div>
            </div>

            <!-- LANZAMIENTOS -->
            <div class="section-block">
                <h2 class="section-title">los mejores lanzamientos</h2>

                <div class="horizontal-scroll"> <!-- scroll horizontal hecho por mi css -->

                    <div class="game-card">
                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/2050650/header.jpg">
                        <div class="game-body">
                            <p class="game-title">Street Fighter 6</p>
                            <span class="price-tag">$59.99</span>
                        </div>
                    </div>

                    <div class="game-card">
                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/990080/header.jpg">
                        <div class="game-body">
                            <p class="game-title">Hogwarts Legacy</p>
                            <span class="price-tag">$59.99</span>
                        </div>
                    </div>

                    <div class="game-card">
                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/1938090/header.jpg">
                        <div class="game-body">
                            <p class="game-title">Call of Duty</p>
                            <span class="price-tag">$69.99</span>
                        </div>
                    </div>

                    <div class="game-card">
                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/686810/header.jpg">
                        <div class="game-body">
                            <p class="game-title">Hell Let Loose</p>
                            <span class="price-tag">$39.99</span>
                        </div>
                    </div>

                    <div class="game-card">
                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/1085660/header.jpg">
                        <div class="game-body">
                            <p class="game-title">Destiny 2</p>
                            <span class="price-tag">free to play</span>
                        </div>
                    </div>

                </div>
            </div>

            <!-- VR -->
            <div class="section-block">
                <div class="d-flex justify-content-between align-items-center mb-2">
                    <h2 class="section-title mb-0">realidad virtual</h2>
                    <a href="#" class="btn btn-sm btn-outline-info">ver todos</a>
                </div>

                <div class="horizontal-scroll"> <!-- scroll manual horizontal -->

                    <div class="game-card">
                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/250820/header.jpg">
                        <div class="game-body">
                            <p class="game-title">SteamVR</p>
                            <span class="price-tag">free</span>
                        </div>
                    </div>

                    <div class="game-card">
                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/546560/header.jpg">
                        <div class="game-body">
                            <p class="game-title">Half-Life: Alyx</p>
                            <span class="price-tag">$59.99</span>
                        </div>
                    </div>

                    <div class="game-card">
                        <img src="https://cdn.akamai.steamstatic.com/steam/apps/648800/header.jpg">
                        <div class="game-body">
                            <p class="game-title">Raft VR Mod</p>
                            <span class="price-tag">$19.99</span>
                        </div>
                    </div>

                </div>
            </div>

        </div>
    </div>

    <!-- FOOTER -->
    <footer>
        <div class="container"> <!-- container bootstrap pa centrar -->
            <div class="row"> <!-- fila -->

                <div class="col-md-3 mb-3">
                    <strong>STIM</strong><br>
                    Proyecto académico tipo Steam.<br>
                    Los nombres de juegos pertenecen a sus dueños.
                </div>

                <div class="col-md-6 mb-3 text-center footer-links">
                    <a href="#">acerca de stim</a>
                    <a href="#">empleo</a>
                    <a href="#">distribución</a>
                    <a href="#">soporte</a>
                    <a href="#">tarjetas regalo</a>
                </div>

                <div class="col-md-3 mb-3 text-end"> <!-- alineación derecha con bootstrap -->
                    © 2025 STIM INTERACTIVE
                </div>

            </div>
        </div>
    </footer>

    <!-- Bootstrap JS -->
    <script
      src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
    ></script> <!-- script de bootstrap pa que funcione el carrusel y el menú -->

</body>
</html>

```
## **estilos.css**


```html
/* el body entero de la pag — aqui ponemos el color de fondo estilo steam
   y la fuente general de toda la pagina */
body {
    background-color: #1b2838;
    color: #c7d5e0;
    font-family: Arial, Helvetica, sans-serif;
}

a {
    text-decoration: none; /* links sin subrayado porque asi se ve mejor */
}

/* barra superior negra (instalar stim, usuario, etc)
   esta barra es la que está arriba de todo tipo steam real */
.top-bar {
    background-color: #000000;
    color: #b8b6b4;
    font-size: 13px;
    padding: 6px 0;
}

.top-bar a {
    color: #b8b6b4;
}

.top-bar a:hover {
    color: #ffffff; /* al poner el mouse se pone blanco como steam */
}

/* navbar principal — aqui usamos bootstrap para el navbar
   (la parte del menu grande donde estan tienda, categorias, etc)
   bootstrap nos da la estructura y nosotros sólo le cambiamos los colores */
.main-nav {
    background-color: #171a21;
}

.main-nav .navbar-brand {
    font-weight: 700;
    letter-spacing: 1px;
}

.main-nav .nav-link {
    color: #c7d5e0 !important;
    font-size: 14px;
    margin-right: 10px;
}

.main-nav .nav-link.active,
.main-nav .nav-link:hover {
    color: #66c0f4 !important;
}

/* contenedor general que envuelve todo el contenido debajo del navbar */
.content-wrap {
    background-color: #1b2838;
    padding-bottom: 40px;
}

/* bloques grandes tipo tarjetas (banner, recomendados, categorias, etc)
   estos son como "secciones" estilo steam */
.section-block {
    background-color: #16202d;
    padding: 20px 25px;
    border-radius: 4px;
    margin-bottom: 25px;
}

.section-title {
    font-size: 22px;
    font-weight: 700;
    margin-bottom: 15px;
}

/* banner principal (la imagen grande con un boton) */
.hero-banner {
    position: relative;
    overflow: hidden;
    border-radius: 4px;
}

.hero-banner img {
    width: 100%;
    display: block; /* sin espacios raros abajo */
}

/* texto que va encima del banner
   por eso usamos position absolute para montarlo arriba */
.hero-info {
    position: absolute;
    left: 20px;
    bottom: 20px;
    max-width: 350px;
}

/* etiqueta pequeña negra trasparente tipo “survival — accion — open world” */
.hero-tag {
    background: rgba(0, 0, 0, 0.6);
    display: inline-block;
    padding: 4px 8px;
    font-size: 12px;
    margin-bottom: 5px;
}

/* boton azul del banner */
.hero-btn {
    background: #0479bb;
    border: none;
    padding: 8px 20px;
    color: #fff;
}

.hero-btn:hover {
    background: #18a0ff;
}

/* tarjetas de juegos (las cartitas con imagen + precio)
   aqui usamos bootstrap para columnas y grid, pero el diseño visual es nuestro */
.game-card {
    background-color: #2a475e;
    border: none;
    border-radius: 3px;
    overflow: hidden;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.game-card:hover {
    transform: scale(1.03);
    box-shadow: 0 0 15px rgba(0,0,0,.5);
}

.game-card img {
    width: 100%;
}

.game-body {
    padding: 8px 10px 10px;
    font-size: 13px;
}

.game-title {
    font-weight: 600;
    margin-bottom: 4px;
}

/* precio final */
.price-tag {
    background-color: #4c6b22;
    color: #fff;
    padding: 2px 6px;
    border-radius: 2px;
    font-weight: 700;
    font-size: 12px;
}

/* descuento en verde */
.discount {
    color: #a4d007;
    font-weight: 700;
    margin-right: 6px;
    font-size: 13px;
}

/* precio antiguo tachado */
.old-price {
    text-decoration: line-through; /* esto es para tacharlo */
    color: #738895;
    font-size: 11px;
}

/* categorias (las tarjetitas azules de generos) */
.category-card {
    background-color: #2a475e;
    border-radius: 3px;
    overflow: hidden;
    transition: transform 0.2s ease;
}

.category-card:hover {
    transform: scale(1.02);
}

.category-name {
    text-align: center;
    padding: 8px 0;
    font-weight: 600;
}

/* scroll horizontal estilo steam
   esto sirve para las tarjetas que se mueven de izquierda a derecha */
.horizontal-scroll {
    overflow-x: auto;
    white-space: nowrap;
}

.horizontal-scroll .game-card {
    display: inline-block;
    width: 260px;
    margin-right: 10px;
}

/* footer estilo steam */
footer {
    background-color: #171a21;
    color: #8f98a0;
    font-size: 12px;
}

---

## **5. Resultado final esperado**

La página final se ve similar a:

<img width="1200" height="933" alt="image" src="https://github.com/user-attachments/assets/ded9f475-bfc6-42ce-91d0-844001c27fb7" />
<img width="1175" height="849" alt="image" src="https://github.com/user-attachments/assets/7768e608-959f-4e8d-aadb-f6eaca70b7bc" />

