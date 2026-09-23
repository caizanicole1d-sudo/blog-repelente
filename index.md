<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Uso adecuado del repelente para mosquitos</title>

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

        /* ================= MENÚ ================= */

        nav {
            position: sticky;
            top: 0;
            z-index: 1000;
            background: rgba(255,255,255,0.97);
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


        /* ================= PORTADA ================= */

        .hero {
            min-height: 650px;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 80px 25px;

            background:
                linear-gradient(
                    rgba(31, 67, 49, 0.82),
                    rgba(31, 67, 49, 0.82)
                ),
                linear-gradient(135deg, #789681, #d8dfd3);

            color: white;
        }

        .hero-content {
            max-width: 950px;
        }

        .school {
            font-size: 15px;
            letter-spacing: 2px;
            line-height: 1.8;
            margin-bottom: 35px;
            text-transform: uppercase;
        }

        .project {
            font-size: 13px;
            letter-spacing: 4px;
            text-transform: uppercase;
            margin-bottom: 20px;
            color: #f0d9a7;
        }

        .hero h1 {
            font-size: clamp(42px, 7vw, 76px);
            line-height: 1.05;
            margin-bottom: 35px;
            font-weight: 700;
        }

        .student-info {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 15px;
            max-width: 900px;
            margin: 35px auto 0;
        }

        .info-box {
            background: rgba(255,255,255,0.12);
            border: 1px solid rgba(255,255,255,0.25);
            border-radius: 15px;
            padding: 18px 12px;
            backdrop-filter: blur(5px);
        }

        .info-box strong {
            display: block;
            color: #f0d9a7;
            font-size: 11px;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 5px;
        }

        .info-box span {
            font-size: 15px;
        }


        /* ================= SECCIONES ================= */

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


        /* ================= TARJETAS ================= */

        .cards {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .card {
            background: white;
            padding: 32px;
            min-height: 190px;
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


        /* ================= BLOQUES DESTACADOS ================= */

        .highlight {
            background: #294333;
            color: white;
            border-radius: 30px;
            padding: 65px;
            text-align: center;
            box-shadow: 0 15px 35px rgba(30,55,40,0.18);
        }

        .highlight h2 {
            font-size: 40px;
            margin-bottom: 15px;
        }


        /* ================= GALERÍA ================= */

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


        /* ================= OPINIÓN ================= */

        .opinion {
            background: #e6eee4;
            border-radius: 30px;
            padding: 65px;
            min-height: 220px;
        }


        /* ================= FUENTES ================= */

        .sources {
            background: white;
            border-radius: 25px;
            padding: 35px;
            min-height: 150px;
            box-shadow: 0 8px 25px rgba(40,60,45,0.07);
        }


        /* ================= FOOTER ================= */

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


        /* ================= CELULAR ================= */

        @media (max-width: 800px) {

            nav {
                gap: 3px;
            }

            nav a {
                font-size: 12px;
                padding: 7px 9px;
            }

            .hero {
                min-height: 600px;
            }

            .student-info {
                grid-template-columns: 1fr 1fr;
            }

            .cards {
                grid-template-columns: 1fr;
            }

            .gallery {
                grid-template-columns: 1fr;
            }

            .highlight {
                padding: 45px 25px;
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

        <div class="school">
            UNIDAD EDUCATIVA DE LAS FUERZAS ARMADAS<br>
            LICEO NAVAL DE GUAYAQUIL<br>
            «CMDTE. RAFAEL ANDRADE LALAMA»
        </div>

        <div class="project">
            Proyecto interdisciplinario
        </div>

        <h1>
            Uso adecuado del<br>
            repelente para mosquitos
        </h1>


        <div class="student-info">

            <div class="info-box">
                <strong>Estudiante</strong>
                <span>Caiza Nicole</span>
            </div>

            <div class="info-box">
                <strong>Curso y paralelo</strong>
                <span>1ro Delta</span>
            </div>

            <div class="info-box">
                <strong>Docente responsable</strong>
                <span>Génesis Rivera</span>
            </div>

            <div class="info-box">
                <strong>Fecha</strong>
                <span>22 de septiembre de 2026</span>
            </div>

        </div>

    </div>

</header>



<!-- ================= PRESENTACIÓN ================= -->

<section id="presentacion">

    <div class="section-title">

        <span>01 · Presentación</span>

        <h2>Presentación del proyecto</h2>

    </div>


    <div class="cards">

        <div class="card">

            <div class="icon">🦟</div>

            <h3>Uso adecuado del repelente</h3>

        </div>


        <div class="card">

            <div class="icon">🎯</div>

            <h3>Proyecto interdisciplinario</h3>

        </div>


        <div class="card">

            <div class="icon">🌿</div>

            <h3>Liceo Naval de Guayaquil</h3>

        </div>

    </div>

</section>



<!-- ================= INVESTIGACIÓN ================= -->

<section id="investigacion">

    <div class="section-title">

        <span>02 · Investigación</span>

        <h2>Investigación</h2>

    </div>


    <div class="cards">

        <div class="card">
            <div class="icon">🔬</div>
            <h3>Investigación científica</h3>
        </div>

        <div class="card">
            <div class="icon">📖</div>
            <h3>Información del tema</h3>
        </div>

        <div class="card">
            <div class="icon">💡</div>
            <h3>Datos importantes</h3>
        </div>

    </div>

</section>



<!-- ================= MATERIALES ================= -->

<section id="materiales">

    <div class="highlight">

        <h2>🧪 Materiales</h2>

    </div>

</section>



<!-- ================= EVIDENCIAS ================= -->

<section id="evidencias">

    <div class="section-title">

        <span>04 · Evidencias</span>

        <h2>Evidencias del proyecto</h2>

    </div>


    <div class="gallery">

        <div class="photo">
            📷<br>
            Evidencia 1
        </div>

        <div class="photo">
            📷<br>
            Evidencia 2
        </div>

        <div class="photo">
            📷<br>
            Evidencia 3
        </div>

        <div class="photo">
            📷<br>
            Evidencia 4
        </div>

        <div class="photo">
            📷<br>
            Evidencia 5
        </div>

        <div class="photo">
            📷<br>
            Evidencia 6
        </div>

    </div>

</section>



<!-- ================= PRODUCTO ================= -->

<section id="producto">

    <div class="highlight">

        <h2>🌿 Nuestro producto</h2>

    </div>

</section>



<!-- ================= OPINIÓN ================= -->

<section id="opinion">

    <div class="section-title">

        <span>07 · Opinión</span>

        <h2>Artículo de opinión</h2>

    </div>


    <div class="opinion">

    </div>

</section>



<!-- ================= CONCLUSIONES ================= -->

<section id="conclusiones">

    <div class="section-title">

        <span>08 · Conclusiones</span>

        <h2>Conclusiones</h2>

    </div>


    <div class="cards">

        <div class="card">

            <div class="icon">✓</div>

            <h3>Conclusión 1</h3>

        </div>


        <div class="card">

            <div class="icon">✓</div>

            <h3>Conclusión 2</h3>

        </div>


        <div class="card">

            <div class="icon">✓</div>

            <h3>Conclusión 3</h3>

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

    </div>

</section>



<!-- ================= PIE DE PÁGINA ================= -->

<footer>

    <h3>
        Uso adecuado del repelente para mosquitos
    </h3>

    <p>
        Unidad Educativa de las Fuerzas Armadas ·
        Liceo Naval de Guayaquil
    </p>

</footer>


</body>
</html>
