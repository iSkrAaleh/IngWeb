

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

<!-- Bootstrap: sirve para usar grillas, navbar, botones, carruseles, etc -->
<link
href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
rel="stylesheet">

<!-- Enlace a mis estilos personalizados -->
<link rel="stylesheet" href="estilos/estilos.css">

</head>
<body>

<!-- TOP BAR (barra superior estilo Steam) -->
<div class="top-bar">
    <div class="container d-flex justify-content-between align-items-center">
            
        <div>
            <span class="me-3">STIM</span> <!-- Nombre de la página -->
            <a href="#">tienda</a> |
            <a href="#">comunidad</a> |
            <a href="#">acerca de</a>
        </div>

        <div>
            <a href="#" class="me-3">instalar stim</a> <!-- Enlace tipo Steam -->
            <a href="#" class="me-2">iniciar sesion</a>
            <span>$cero dolare USD</span> <!-- saldo falso -->
        </div>

    </div>
</div>

<!-- NAVBAR PRINCIPAL (responsive gracias a Bootstrap) -->
<nav class="navbar navbar-expand-lg navbar-dark main-nav">

    <div class="container">

        <a class="navbar-brand" href="#">STIM</a> <!-- Logo grande -->

        <!-- Botón hamburguesa para pantallas pequeñas -->
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#mainMenu">
            <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="mainMenu">

            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                <li class="nav-item"><a class="nav-link active" href="#">TIENDA</a></li>
                <li class="nav-item"><a class="nav-link" href="#">COMUNIDAD</a></li>
                <li class="nav-item"><a class="nav-link" href="#">CHAT</a></li>
                <li class="nav-item"><a class="nav-link" href="#">SOPORTE</a></li>
            </ul>

            <!-- Buscador -->
            <form class="d-flex" role="search">
                <input class="form-control form-control-sm me-2" type="search" placeholder="buscar en la tienda">
                <button class="btn btn-sm btn-outline-info" type="submit">buscar</button>
            </form>

        </div>
    </div>
</nav>

<!-- CONTENIDO GENERAL -->
<div class="content-wrap">
<div class="container py-4">

<!-- BANNER PRINCIPAL -->
<div class="section-block hero-banner mb-4">

    <img src="https://cdn.akamai.steamstatic.com/steam/apps/1938090/library_hero.jpg"> <!-- Imagen grande -->

    <div class="hero-info">
        <span class="hero-tag">ya disponible</span>
        <h1>CALL OF DUTY BLACK OPS</h1>
        <p class="mb-2">Vive una nueva campaña, modos multijugador y experiencia zombies.</p>
        <button class="hero-btn">ver en stim</button>
    </div>
</div>

<!-- SECCIÓN DESTACADOS -->
<div class="section-block">

    <div class="d-flex justify-content-between align-items-center mb-2">
        <h2 class="section-title mb-0">destacados y recomendados</h2>
    </div>

<!-- CAROUSEL -->
<div id="carouselDestacados" class="carousel slide" data-bs-ride="carousel">

<div class="carousel-inner">

    <!-- SLIDE 1 -->
    <div class="carousel-item active">
        <div class="row g-3">

            <div class="col-md-3">
                <div class="game-card">
                    <img src="https://cdn.akamai.steamstatic.com/steam/apps/1091500/header.jpg">
                    <div class="game-body">
                        <p class="game-title">Cyberpunk 2077</p>
                        <span class="discount">-50%</span>
                        <span class="old-price">$59.99</span>
                        <span class="price-tag">$29.99</span>
                    </div>
                </div>
            </div>

        </div>
    </div>

    <!-- SLIDE 2 -->
    <div class="carousel-item">
        <div class="row g-3">
            <!-- tarjetas del segundo slide -->
        </div>
    </div>

</div>

<!-- BOTÓN IZQUIERDA -->
<button class="carousel-control-prev" type="button"
data-bs-target="#carouselDestacados" data-bs-slide="prev">
    <span class="carousel-control-prev-icon"></span>
</button>

<!-- BOTÓN DERECHA -->
<button class="carousel-control-next" type="button"
data-bs-target="#carouselDestacados" data-bs-slide="next">
    <span class="carousel-control-next-icon"></span>
</button>

</div>
</div>

</div>
</div>

<!-- Scripts necesarios de Bootstrap -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>

</body>
</html>
```

---

## 🎨 **estilos.css**

```css
/* color de fondo general y fuente principal */
body {
background-color: #1b2838;   /* azul oscuro estilo Steam */
color: #c7d5e0;               /* texto azul claro */
font-family: Arial, Helvetica, sans-serif;
}

a {
text-decoration: none; /* sin subrayado */
}

/* BARRA SUPERIOR */
.top-bar {
background-color: #000000; /* negro */
color: #b8b6b4;            /* gris claro */
font-size: 13px;
padding: 6px 0;
}

.top-bar a { color: #b8b6b4; }
.top-bar a:hover { color: #ffffff; }

/* NAVBAR PRINCIPAL */
.main-nav {
background-color: #171a21; /* color de Steam */
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
color: #66c0f4 !important; /* azul hover */
}

/* CONTENIDO GENERAL */
.content-wrap {
background-color: #1b2838;
padding-bottom: 40px;
}

/* TARJETAS / SECCIONES */
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

/* BANNER PRINCIPAL */
.hero-banner {
position: relative;
overflow: hidden;
border-radius: 4px;
}

.hero-banner img {
width: 100%;
display: block;
}

.hero-info {
position: absolute;
left: 20px;
bottom: 20px;
max-width: 350px;
}

.hero-tag {
background: rgba(0, 0, 0, 0.6);
padding: 4px 8px;
font-size: 12px;
}

.hero-btn {
background: #0479bb;
border: none;
padding: 8px 20px;
color: #fff;
}

.hero-btn:hover {
background: #18a0ff;
}

/* TARJETAS DE JUEGOS */
.game-card {
background-color: #2a475e;
border: none;
border-radius: 3px;
overflow: hidden;
transition: transform .2s, box-shadow .2s;
}

.game-card:hover {
transform: scale(1.03);
box-shadow: 0 0 15px rgba(0,0,0,.5);
}

.game-card img { width: 100%; }

.game-body {
padding: 8px 10px;
font-size: 13px;
}

.game-title {
font-weight: 600;
margin-bottom: 4px;
}

.price-tag {
background-color: #4c6b22;
color: #fff;
padding: 2px 6px;
border-radius: 2px;
font-weight: 700;
}

.discount {
color: #a4d007;
font-weight: 700;
margin-right: 6px;
}

.old-price {
text-decoration: line-through;
color: #738895;
font-size: 11px;
}

/* CATEGORÍAS */
.category-card {
background-color: #2a475e;
border-radius: 3px;
transition: transform .2s;
}

.category-card:hover {
transform: scale(1.02);
}

.category-name {
text-align: center;
padding: 8px 0;
font-weight: 600;
}

/* SCROLL HORIZONTAL */
.horizontal-scroll {
overflow-x: auto;
white-space: nowrap;
}

.horizontal-scroll .game-card {
display: inline-block;
width: 260px;
margin-right: 10px;
}

/* FOOTER */
footer {
background-color: #171a21;
color: #8f98a0;
font-size: 12px;
}
```

---

## **5. Resultado final esperado**

La página final se ve similar a:

<img width="1200" height="933" alt="image" src="https://github.com/user-attachments/assets/ded9f475-bfc6-42ce-91d0-844001c27fb7" />
<img width="1175" height="849" alt="image" src="https://github.com/user-attachments/assets/7768e608-959f-4e8d-aadb-f6eaca70b7bc" />

