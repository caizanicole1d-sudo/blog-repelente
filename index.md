<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Uso adecuado del repelente</title>

    <style>

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: "Segoe UI", Arial, sans-serif;
            background: #f5f3ec;
            color: #26352d;
            line-height: 1.7;
        }

        /* ---------- MENÚ ---------- */

        nav {
            position: sticky;
            top: 0;
            z-index: 1000;
            background: rgba(255,255,255,0.96);
            backdrop-filter: blur(10px);
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
            gap: 8px;
            padding: 16px 20px;
            box-shadow: 0 3px 15px rgba(0,0,0,0.08);
        }

        nav a {
            text-decoration: none;
            color: #365342;
            font-size: 14px;
            font-weight: 600;
            padding: 9px 14px;
            border-radius: 20px;
            transition: 0.3s;
        }

        nav a:hover {
            background: #dce8dd;
            color: #183a27;
        }


        /* ---------- PORTADA ---------- */

        .hero {
            min-height: 600px;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 80px 25px;
            background:
                linear-gradient(
                    rgba(31, 67, 49, 0.78),
                    rgba(31, 67, 49, 0.78)
                ),
                linear-gradient(135deg, #789681, #d8dfd3);
            color: white;
        }

        .hero-content {
            max-width: 900px;
        }

        .small-title {
            letter-spacing: 4px;
            text-transform: uppercase;
            font-size: 13px;
            margin-bottom: 20px;
            opacity: 0.9;
        }

        .hero h1 {
            font-size: clamp(42px, 7vw, 76px);
            line-height: 1.05;
            margin-bottom: 25px;
            font-weight: 700;
        }

        .hero p {
            font-size: 20px;
            max-width: 650px;
            margin: auto;
            opacity: 0.95;
        }

        .hero-button {
            display: inline-block;
            margin-top: 35px;
            padding: 14px 28px;
            background: #f0d9a7;
            color: #294333;
            text-decoration: none;
            border-radius: 30px;
            font-weight: bold;
            transition: 0.3s;
        }

        .hero-button:hover {
            transform: translateY(-3px);
            background: #fff0c9;
        }


        /* ---------- SECCIONES ---------- */

        section {
            max-width: 1100px;
            margin: auto;
            padding: 90px 25px;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title span {
            display: block;
            color: #789681;
            text-transform: uppercase;
            letter-spacing: 3px;
            font-size: 12px;
            font-weight: bold;
            margin-bottom: 8px;
        }

        .section-title h2 {
            font-size: 38px;
            color: #294333;
        }

        .section-title p {
            max-width: 650px;
            margin: 12px auto 0;
            color: #68736c;
        }


        /* ---------- TARJETAS ---------- */

        .cards {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .card {
            background: white;
            padding: 32px;
            border-radius: 20px;
            box-shadow: 0 8px 25px rgba(40,60,45,0.08);
            transition: 0.3s;
            border: 1px solid #e7ebe5;
        }

        .card:hover {
            transform: translateY(-7px);
            box-shadow: 0 15px 30px rgba(40,60,45,0.13);
        }

        .icon {
            width: 55px;
            height: 55px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 15px;
            background: #e2ebe1;
            font-size: 25px;
            margin-bottom: 20px;
        }

        .card h3 {
            color: #294333;
            margin-bottom: 10px;
        }

        .card p {
            color: #68736c;
        }


        /* ---------- BLOQUE DESTACADO ---------- */

        .highlight {
            background: #294333;
            color: white;
            border-radius: 30px;
            padding: 60px;
            text-align: center;
            box-shadow: 0 15px 35px rgba(30,55,40,0.18);
        }

        .highlight h2 {
            font-size: 40px;
            margin-bottom: 15px;
        }

        .highlight p {
            max-width: 700px;
            margin: auto;
            color: #e5eee6;
        }


        /* ---------- GALERÍA ---------- */

        .gallery {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .photo {
            height: 240px;
            border-radius: 20px;
            background: linear-gradient(135deg, #d9e3d8, #edf0e9);
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: #657269;
            font-weight: 600;
            border: 2px dashed #b8c7b8;
            transition: 0.3s;
        }

        .photo:hover {
            transform: scale(1.02);
        }


        /* ---------- OPINIÓN ---------- */

        .opinion {
            background: #e6eee4;
            border-radius: 30px;
            padding: 55px;
            text-align: center;
        }

        .opinion p {
            max-width: 750px;
            margin: auto;
            font-size: 19px;
            color: #4d5d51;
        }


        /* ---------- FUENTES ---------- */

        .sources {
            background: white;
            border-radius: 25px;
            padding: 35px;
            box-shadow: 0 8px 25px rgba(40,60,45,0.07);
        }

        .sources ul {
            padding-left: 25px;
        }

        .sources li {
            margin: 10px 0;
        }


        /* ---------- FOOTER ---------- */

        footer {
            background: #1e3025;
            color: white;
            text-align: center;
            padding: 45px 20px;
        }

        footer h3 {
            margin-bottom: 10px;
            font-size: 22px;
        }

        footer p {
            color: #cbd7cd;
        }


        /* ---------- CELULAR ---------- */

        @media (max-width: 800px) {

            nav {
                gap: 3px;
            }

            nav a {
                font-size: 12px;
                padding: 7px 9px;
            }

            .hero {
                min-height: 500px;
            }

            .cards {
                grid-template-columns: 1fr;
            }

            .gallery {
                grid-template-columns: 1fr;
            }

            .highlight {
                padding: 40px 25px;
            }

            .opinion {
                padding: 40px 25px;
            }

            section {
                padding: 65px 20px;
            }
        }

    </style>
</head>


<body>


<!-- ================= MENÚ ================= -->

<nav>

    <a href="#inicio">Inicio</a>

    <a href="#presentacion">Presentación</a>

    <a href="#investigacion">Investigación</a>

    <a href="#materiales">Materiales</a>

    <a href="#evidencias">Evidencias</a>

    <a href="#producto">Producto</a>

    <a href="#opinion">Opinión</a>

    <a href="#conclusiones">Conclusiones</a>

    <a href="#fuentes">Fuentes</a>

</nav>



<!-- ================= PORTADA ================= -->

<header class="hero" id="inicio">

    <div class="hero-content">

        <div class="small-title">
            Proyecto interdisciplinario
        </div>

        <h1>
            Uso adecuado del<br>
            repelente para mosquitos
        </h1>

        <p>
            Un proyecto para conocer, investigar y experimentar
            sobre la protección frente a los mosquitos.
        </p>

        <a href="#presentacion" class="hero-button">
            Conocer el proyecto
        </a>

    </div>

</header>



<!-- ================= PRESENTACIÓN ================= -->

<section id="presentacion">

    <div class="section-title">

        <span>01 · Presentación</span>

        <h2>Conociendo nuestro proyecto</h2>

        <p>
            Aquí irá la presentación general del proyecto.
        </p>

    </div>


    <div class="cards">

        <div class="card">

            <div class="icon">🦟</div>

            <h3>Tema</h3>

            <p>
                Espacio reservado para explicar el tema principal.
            </p>

        </div>


        <div class="card">

            <div class="icon">🎯</div>

            <h3>Objetivo</h3>

            <p>
                Aquí colocaremos el objetivo del proyecto.
            </p>

        </div>


        <div class="card">

            <div class="icon">🌿</div>

            <h3>Importancia</h3>

            <p>
                Aquí explicaremos por qué es importante este proyecto.
            </p>

        </div>

    </div>

</section>



<!-- ================= INVESTIGACIÓN ================= -->

<section id="investigacion">

    <div class="section-title">

        <span>02 · Investigación</span>

        <h2>Lo que aprendimos</h2>

        <p>
            En esta sección irá la información investigada.
        </p>

    </div>


    <div class="cards">

        <div class="card">

            <div class="icon">🔬</div>

            <h3>Investigación</h3>

            <p>
                Aquí irá la información científica del proyecto.
            </p>

        </div>


        <div class="card">

            <div class="icon">📖</div>

            <h3>Conceptos importantes</h3>

            <p>
                Aquí colocaremos las definiciones necesarias.
            </p>

        </div>


        <div class="card">

            <div class="icon">💡</div>

            <h3>Datos importantes</h3>

            <p>
                Aquí se colocarán los datos obtenidos durante la investigación.
            </p>

        </div>

    </div>

</section>



<!-- ================= MATERIALES ================= -->

<section id="materiales">

    <div class="highlight">

        <h2>🧪 Materiales</h2>

        <p>
            En este espacio colocaremos los materiales utilizados
            para elaborar nuestro producto.
        </p>

    </div>

</section>



<!-- ================= EVIDENCIAS ================= -->

<section id="evidencias">

    <div class="section-title">

        <span>04 · Evidencias</span>

        <h2>Nuestro proceso</h2>

        <p>
            Aquí aparecerán las fotografías del proceso del proyecto.
        </p>

    </div>


    <div class="gallery">

        <div class="photo">
            📷<br>
            Foto del proceso 1
        </div>

        <div class="photo">
            📷<br>
            Foto del proceso 2
        </div>

        <div class="photo">
            📷<br>
            Foto del proceso 3
        </div>

        <div class="photo">
            📷<br>
            Foto del proceso 4
        </div>

        <div class="photo">
            📷<br>
            Foto del proceso 5
        </div>

        <div class="photo">
            📷<br>
            Foto del proceso 6
        </div>

    </div>

</section>



<!-- ================= PRODUCTO ================= -->

<section id="producto">

    <div class="highlight">

        <h2>🌿 Nuestro producto</h2>

        <p>
            Aquí presentaremos el repelente elaborado,
            su preparación y sus características.
        </p>

    </div>

</section>



<!-- ================= OPINIÓN ================= -->

<section id="opinion">

    <div class="section-title">

        <span>07 · Opinión</span>

        <h2>Nuestra experiencia</h2>

    </div>


    <div class="opinion">

        <p>
            Aquí colocaremos nuestra opinión y experiencia
            durante la realización del proyecto.
        </p>

    </div>

</section>



<!-- ================= CONCLUSIONES ================= -->

<section id="conclusiones">

    <div class="section-title">

        <span>08 · Conclusiones</span>

        <h2>Lo que nos llevamos</h2>

        <p>
            Aquí colocaremos las conclusiones finales del proyecto.
        </p>

    </div>


    <div class="cards">

        <div class="card">

            <div class="icon">✓</div>

            <h3>Conclusión 1</h3>

            <p>
                Espacio reservado para la primera conclusión.
            </p>

        </div>


        <div class="card">

            <div class="icon">✓</div>

            <h3>Conclusión 2</h3>

            <p>
                Espacio reservado para la segunda conclusión.
            </p>

        </div>


        <div class="card">

            <div class="icon">✓</div>

            <h3>Conclusión 3</h3>

            <p>
                Espacio reservado para la tercera conclusión.
            </p>

        </div>

    </div>

</section>



<!-- ================= FUENTES ================= -->

<section id="fuentes">

    <div class="section-title">

        <span>09 · Fuentes</span>

        <h2>Fuentes consultadas</h2>

    </div>


    <div class="sources">

        <ul>

            <li>Fuente 1 — pendiente de agregar.</li>

            <li>Fuente 2 — pendiente de agregar.</li>

            <li>Fuente 3 — pendiente de agregar.</li>

        </ul>

    </div>

</section>



<!-- ================= PIE ================= -->

<footer>

    <h3>Uso adecuado del repelente para mosquitos</h3>

    <p>
        Proyecto interdisciplinario · Liceo Naval de Guayaquil
    </p>

</footer>


</body>
</html>
