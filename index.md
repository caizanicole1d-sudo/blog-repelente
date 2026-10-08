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
                <span></span>
            </div>

            <div class="info-box">
                <strong>Fecha</strong>
                <span>22 de septiembre de 2026</span>
            </div>

        </div>

    </div>

</header>



<!-- ================= SECCIÓN 01 ================= -->

<section id="presentacion">

    <div class="section-number">
        SECCION 01
    </div>

    <h2>Presentación del proyecto</h2>

    <div class="presentation">

        <p>
            Este proyecto surge a partir de una inquietud común que surgió durante la clase:
            aunque la mayoría de nosotros hemos aplicado repelente más de una vez,
            ¿realmente le damos el uso correcto? Con ese interrogante en mente, el grupo de
            Primero de Bachillerato asumió el reto de indagar, contrastar datos de instituciones
            de salud y elaborar una guía accesible que enseñe a la comunidad a prevenir de
            manera adecuada las picaduras de mosquitos.
        </p>

        <p>
            Seleccionamos este tema debido a las condiciones climáticas de Guayaquil, una
            ciudad caracterizada por su ambiente cálido y lluvioso que propicia la
            acumulación de mosquitos en cualquier época. Ante esta realidad, el repelente deja
            de ser un artículo opcional para convertirse en una medida indispensable de
            protección diaria, útil tanto en los hogares como en la unidad educativa y en
            espacios abiertos.
        </p>

        <p>
            Comprender su correcta aplicación es fundamental, ya que un uso inadecuado
            compromete su efectividad e incluso puede provocar reacciones indeseadas. Por
            ello, nos enfocamos en sintetizar la información de fuentes especializadas y
            plasmarla en un formato claro y práctico, pensado para que cualquier estudiante
            o familiar pueda ponerlo en práctica fácilmente.
        </p>

        <p>
            A través de este trabajo nos planteamos tres metas principales:
        </p>

        <div class="goals">

            <div class="goal">
                <h3>01</h3>
                <p>
                    Desarrollar un criterio analítico para identificar información científica
                    confiable.
                </p>
            </div>

            <div class="goal">
                <h3>02</h3>
                <p>
                    Promover una cultura de cuidado y salud preventiva en nuestro entorno
                    escolar.
                </p>
            </div>

            <div class="goal">
                <h3>03</h3>
                <p>
                    Crear una herramienta perdurable que sirva de apoyo a futuras
                    promociones de estudiantes.
                </p>
            </div>

        </div>

        <div class="phrase">
            «Protegernos correctamente no es solo aplicarnos un producto, sino conocer cómo
            cuidar nuestra salud con responsabilidad.»
            <br><br>
            <strong>Equipo de investigación, 1.º BGU</strong>
        </div>

    </div>

</section>


<!-- ================= SECCIÓN 02 ================= -->

<section id="investigacion">

    <div class="section-number">
        SECCIÓN 02
    </div>

    <h2>CONOCIENDO EL PROBLEMA</h2>

    <p class="intro">
        Previo a plantear soluciones o sugerencias, estructuramos nuestro análisis
        respondiendo a cuatro preguntas clave. De esta forma garantizamos un enfoque
        metódico y sustentado para nuestro proyecto.
    </p>


    <div class="research-grid">

        <div class="research-card">

            <h3>¿Por qué se realiza esta investigación?</h3>

            <p>
                Las picaduras de insectos sobrepasan la simple molestia cutánea: en nuestra
                región representan el principal vector de contagio de virosis como el dengue.
                Comprender los riesgos biológicos y dominar la aplicación adecuada de barreras
                protectoras es una acción fundamental para salvaguardar el bienestar individual
                y familiar.
            </p>

        </div>


        <div class="research-card">

            <h3>¿Para qué se realiza?</h3>

            <p>
                Buscamos desarrollar un aprendizaje práctico y fomentar hábitos preventivos
                sólidos en nuestra comunidad escolar. Pretendemos que el uso de protección
                corporal se realice con criterios científicos validados por organismos de salud,
                dejando de lado supuestos, mitos o costumbres infundadas.
            </p>

        </div>


        <div class="research-card">

            <h3>¿Bajo qué contexto se realiza?</h3>

            <p>
                El entorno de Guayaquil combina elevadas temperaturas con alta humedad y
                temporadas pluviales que propician la proliferación del vector Aedes aegypti.
                Dentro de este escenario geográfico y en el marco de una institución que fomenta
                la autocuidado y la responsabilidad social, analizar la prevención de picaduras
                resulta indispensable y de gran utilidad práctica.
            </p>

        </div>


        <div class="research-card">

            <h3>¿Qué investigaron los estudiantes?</h3>

            <p>
                Examinamos la composición de las fórmulas repelentes, su mecanismo de acción,
                los momentos oportunos de uso, así como las pautas de seguridad y las
                equivocaciones habituales al aplicarlos. Cada uno de estos tópicos se detalla
                minuciosamente en el siguiente bloque.
            </p>

        </div>

    </div>


    <h2 class="learn-title">
        LO QUE APRENDIMOS, PUNTO POR PUNTO
    </h2>

    <p class="intro">
        Sintetizamos los hallazgos en los siguientes temas clave. 
    </p>


    <div class="point-list">

        <div class="point">

            <strong>01. ¿Qué es un repelente?</strong>

            <p>
                Sustancia o preparado formulado para ahuyentar o desorientar a los insectos,
                evitando que se posen o piquen sobre la superficie cutánea.
            </p>

        </div>


        <div class="point">

            <strong>02. ¿Para qué sirve?</strong>

            <p>
                Actúa como una barrera química preventiva que reduce significativamente el
                contacto con vectores de enfermedades.
            </p>

        </div>


        <div class="point">

            <strong>03. ¿Cómo funciona?</strong>

            <p>
                Bloquea los receptores olfativos del mosquito, impidiendo que detecte el
                dióxido de carbono y el sudor que emite el cuerpo humano.
            </p>

        </div>


        <div class="point">

            <strong>04. ¿Cuándo debe utilizarse?</strong>

            <p>
                Especialmente en las horas de mayor actividad del mosquito (primeras horas de
                la mañana y al atardecer) y al permanecer en espacios abiertos o húmedos.
            </p>

        </div>


        <div class="point">

            <strong>05. ¿Cómo debe aplicarse correctamente?</strong>

            <p>
                Rociando o extendiendo una capa uniforme sobre la piel expuesta y la ropa,
                evitando frotar en exceso o aplicar en lugares cubiertos.
            </p>

        </div>


        <div class="point">

            <strong>06. ¿Qué precauciones deben tenerse?</strong>

            <p>
                No aplicar sobre heridas, ojos o boca, evitar el uso excesivo y mantener fuera
                del alcance de niños pequeños sin supervisión.
            </p>

        </div>


        <div class="point">

            <strong>07. ¿Qué errores deben evitarse?</strong>

            <p>
                Mezclar incorrectamente con protector solar (se debe poner primero el bloqueador
                y luego el repelente), inhalar el producto o usar concentraciones no aptas para la
                edad.
            </p>

        </div>


        <div class="point">

            <strong>08. La importancia de leer la etiqueta</strong>

            <p>
                Revisar las instrucciones permite conocer la concentración del principio activo
                (como DEET o Icaridina), la frecuencia de reaplicación y las edades permitidas.
            </p>

        </div>


        <div class="point">

            <strong>09. Prevención vs. tratamiento: ¿es lo mismo?</strong>

            <p>
                No; la prevención busca evitar la picadura antes de que ocurra, mientras que el
                tratamiento atiende los síntomas (como picazón o inflamación) una vez que el
                insecto ya picó.
            </p>

        </div>

    </div>


    <div class="source-note">

        <strong>Fuente de la información:</strong>

        La información de esta sección fue elaborada a partir de materiales de
        divulgación del Ministerio de Salud Pública del Ecuador, la Organización
        Panamericana de la Salud / OMS, los CDC de Estados Unidos y la Agencia de
        Protección Ambiental (EPA).

    </div>

</section>


<!-- ================= SECCIÓN 03 ================= -->

<section id="materiales">

    <div class="section-number">
        SECCIÓN 03
    </div>

    <h2>MATERIALES DEL PROYECTO</h2>

    <p class="intro">
        Estos fueron los recursos y reactivos utilizados para la experimentación
        y elaboración del prototipo de repelente de origen vegetal.
    </p>


    <div class="materials-grid">

        <div class="material">

            <h3>Repelente para mosquitos</h3>

            <p>
                Producto comercial de referencia empleado como elemento base para la
                comparación de eficacia y la inspección de su etiquetado informativo.
            </p>

        </div>


        <div class="material">

            <h3>Plantas aromáticas</h3>

            <p>
                Muestra vegetal de citronela y hierba luisa,
                utilizadas como insumo activo natural para la extracción
                de aceites esenciales y fragancias.
            </p>

        </div>


        <div class="material">

            <h3>Alcohol antiséptico al 70 %</h3>

            <p>
                Solución a base de etanol empleada como agente extractor del material
                vegetal para disolver y concentrar las sustancias activas de las plantas.
            </p>

        </div>


        <div class="material">

            <h3>Mortero y pistilo</h3>

            <p>
                Instrumento de laboratorio utilizado para triturar y macerar las hojas
                y tallos, facilitando la extracción de los componentes aromáticos.
            </p>

        </div>


        <div class="material">

            <h3>Balanza y probeta</h3>

            <p>
                Equipos de medición para determinar con precisión la masa de las plantas
                (5 g de cada una) y el volumen del solvente (50 mL).
            </p>

        </div>


        <div class="material">

            <h3>Vasos de precipitación y varilla</h3>

            <p>
                Recipientes de cristal y agitador usados para realizar la mezcla, permitir
                el reposo de la extracción y homogeneizar el preparado.
            </p>

        </div>


        <div class="material">

            <h3>Embudo y papel filtro</h3>

            <p>
                Sistema de filtrado para separar los residuos sólidos del extracto líquido
                obtenido durante el proceso de maceración.
            </p>

        </div>


        <div class="material">

            <h3>Frasco con atomizador</h3>

            <p>
                Envase final dosificador que permite almacenar el repelente obtenido y
                aplicarlo de forma uniforme en aerosol.
            </p>

        </div>

    </div>

</section>


<!-- ================= SECCIÓN 04 ================= -->

<section id="evidencias">

    <div class="evidence-content">

        <div class="section-number">
            SECCIÓN 04
        </div>

        <h2>EVIDENCIAS</h2>

        <p class="intro">
            Evidencias del desarrollo del proyecto.
            Haz clic sobre una imagen para verla en tamaño grande.
        </p>


        <div class="stage">

            <h3>Investigación</h3>

            <div class="photos">

                <div class="photo" onclick="abrirImagen('imagenes/evidencia1.jpg')">
                    <img src="imagenes/evidencia1.jpg" alt="Evidencia 1">
                </div>

                <div class="photo" onclick="abrirImagen('imagenes/evidencia2.jpg')">
                    <img src="imagenes/evidencia2.jpg" alt="Evidencia 2">
                </div>

                <div class="photo" onclick="abrirImagen('imagenes/evidencia3.jpg')">
                    <img src="imagenes/evidencia3.jpg" alt="Evidencia 3">
                </div>

            </div>

        </div>


        <div class="stage">

            <h3>Elaboración</h3>

            <div class="photos">

                <div class="photo" onclick="abrirImagen('imagenes/evidencia4.jpg')">
                    <img src="imagenes/evidencia4.jpg" alt="Evidencia 4">
                </div>

                <div class="photo" onclick="abrirImagen('imagenes/evidencia5.jpg')">
                    <img src="imagenes/evidencia5.jpg" alt="Evidencia 5">
                </div>

                <div class="photo" onclick="abrirImagen('imagenes/evidencia6.jpg')">
                    <img src="imagenes/evidencia6.jpg" alt="Evidencia 6">
                </div>

            </div>

        </div>


        <div class="stage">

            <h3>Proceso del proyecto</h3>

            <div class="photos">

                <div class="photo" onclick="abrirImagen('imagenes/evidencia7.jpg')">
                    <img src="imagenes/evidencia7.jpg" alt="Evidencia 7">
                </div>

                <div class="photo" onclick="abrirImagen('imagenes/evidencia8.jpg')">
                    <img src="imagenes/evidencia8.jpg" alt="Evidencia 8">
                </div>

            </div>

        </div>

    </div>

</section>


<!-- ================= SECCIÓN 05 ================= -->

<section id="producto">

    <div class="section-number">
        SECCIÓN 05
    </div>

    <h2>NUESTRO PRODUCTO</h2>

    <div class="product-box">

        <div class="product-image">

            <img
                src="imagenes/producto.jpg"
                alt="Producto elaborado"
            >

        </div>

        <div>

            <h3>Repelente a base de plantas aromáticas</h3>

            <p>
                El proyecto contempla la elaboración de un prototipo de biorepelente
                utilizando material vegetal aromático y alcohol al 70 % como agente
                extractor.
            </p>

            <br>

            <p>
                El producto final se almacena en un frasco con atomizador para facilitar
                su aplicación.
            </p>

        </div>

    </div>

</section>


<!-- ================= SECCIÓN 06 ================= -->

<section id="opinion">

    <div class="opinion-content">

        <div class="section-number">
            SECCIÓN 06 · ARTÍCULO DE OPINIÓN
        </div>

        <h2>NUESTRA OPINIÓN</h2>

        <h3>
            El poder de las plantas: la naturaleza
            como escudo contra los mosquitos
        </h3>

        <p>
            En nuestra vida cotidiana, las picaduras de mosquitos no solo son molestas, sino que
            también representan un peligro para la salud porque pueden transmitir varias
            enfermedades. Para protegernos, casi siempre acudimos a los repelentes, pero es
            importante entender cómo funcionan realmente. A diferencia de los insecticidas, que
            están hechos para matar al insecto, los repelentes son compuestos (químicos o naturales)
            diseñados para evitar que artrópodos como mosquitos, garrapatas o moscas se posen
            sobre la piel o la ropa.
           
        </p>

        <p>
            En este sentido, yo opino que los repelentes a base de plantas naturales son la mejor
            opción para protegernos, ya que logran desorientar los sensores de los mosquitos y
            volvernos "invisibles" para ellos sin necesidad de hacerles daño.
        </p>

        <p>
            En primer lugar, hay que entender que los mosquitos no nos buscan por suerte o
            casualidad. Ellos se orientan usando receptores olfativos que detectan el dióxido de
            carbono (CO2) que expulsamos al respirar, el ácido láctico del sudor y el calor de nuestro
            cuerpo. Cuando aplicamos un biorepelente con extractos de plantas aromáticas (como la
            citronela, el eucalipto o la menta), sus aromas saturan y bloquean estos sensores. Al no
            poder oler nuestras señales químicas, el mosquito se desorienta y la persona se vuelve
            prácticamente "invisible" ante sus sentidos.
        </p>

        <p>
            Por otro lado, a través del trabajo de laboratorio que realizamos con nuestro grupo,
            pudimos comprobar que es muy fácil aprovechar el poder de las plantas. Con pasos
            sencillos como triturar las hojas, extraer sus esencias con alcohol al 70 % y filtrarlas bien,
            logramos obtener un extracto muy concentrado. Además, al combinar dos plantas
            diferentes, los aromas se potencian y el efecto repelente es aún mayor. Esto demuestra que
            no necesitamos usar químicos sintéticos fuertes cuando la propia naturaleza nos da
            soluciones naturales, ecológicas y seguras para la piel.
        </p>

        <p>
            Para terminar, considero que la naturaleza es un verdadero escudo que nos protege de los
            insectos. Aprender a elaborar nuestro propio biorepelente a base de plantas aromáticas
            nos enseña que es posible cuidar nuestra salud de forma natural, previniendo picaduras
            sin tener que matar a los mosquitos ni contaminar nuestro entorno. Apoyar estas
            alternativas naturales es la mejor manera de cuidar de nosotros y del medio ambiente al
            mismo tiempo.
        </p>

    </div>

</section>


<!-- ================= SECCIÓN 07 ================= -->

<section id="conclusiones">

    <div class="section-number">
        SECCIÓN 07
    </div>

    <h2>¿QUÉ APRENDIMOS?</h2>

    <p class="intro">
        Estas son las conclusiones que el equipo obtuvo al cerrar la investigación.
    </p>


    <div class="conclusions">

        <div class="conclusion">

            <div class="conclusion-number">01</div>

            <p>
                Un uso consciente y acertado del repelente transforma un producto
                cotidiano en una barrera efectiva contra insectos, marcando la diferencia
                frente a su aplicación incorrecta o al azar.
            </p>

        </div>


        <div class="conclusion">

            <div class="conclusion-number">02</div>

            <p>
                Revisar detenidamente las indicaciones de la etiqueta es un paso clave para
                garantizar la seguridad, aunque con frecuencia es una práctica ignorada por
                gran parte de la población.
            </p>

        </div>


        <div class="conclusion">

            <div class="conclusion-number">03</div>

            <p>
                La protección integral exige combinar el repelente con otras acciones
                preventivas, como vestir ropa protectora y eliminar los recipientes con agua
                estancada en nuestras viviendas y zonas escolares.
            </p>

        </div>


        <div class="conclusion">

            <div class="conclusion-number">04</div>

            <p>
                Es esencial filtrar la información de salud y validar los datos en entidades
                autorizadas —tales como el Ministerio de Salud Pública, la OPS/OMS o los
                CDC— para evitar mitos y transmitir datos verídicos.
            </p>

        </div>


        <div class="conclusion">

            <div class="conclusion-number">05</div>

            <p>
                El trabajo investigativo en grupo fortaleció nuestro criterio analítico y la
                cooperación, permitiéndonos asumir un rol activo en la promoción de la
                salud dentro de nuestra comunidad.
            </p>

        </div>

    </div>

</section>


<!-- ================= SECCIÓN 08 ================= -->

<section id="fuentes">

    <div class="sources-content">

        <div class="section-number">
            SECCIÓN 08
        </div>

        <h2>FUENTES CONSULTADAS</h2>

        <p>
            Las fuentes utilizadas para la elaboración de la investigación fueron:
        </p>


        <div class="source-list">

            <div class="source">
                <h3>Ministerio de Salud Pública del Ecuador</h3>
                <p>
                   «Ecuador en alerta para prevenir el contagio del dengue»
                   Consultado en 2026 · salud.gob.ec
                </p>
            </div>

            <div class="source">
                <h3>Organización Panamericana de la Salud / OMS</h3>
                <p>
                 «Dengue: síntomas, prevención y tratamiento»
                 Consultado en 2026 · paho.org

                </p>
            </div>

            <div class="source">
                <h3>Centros para el Control y la Prevención de Enfermedades (CDC), EE. UU. </h3>
                <p>
                    «Evite las picaduras de mosquitos» — Especiales CDC en Español
                    Consultado en 2026 · cdc.gov/spanish
                  
                </p>
            </div>

            <div class="source">
                <h3>Centros para el Control y la Prevención de Enfermedades (CDC), EE. UU.</h3>
                <p>
                    «Prevención de picaduras de mosquito» — hoja informativa (PDF)
                    Noviembre 2024 · cdc.gov
                </p>
            </div>

        </div>

    </div>

</section>


<!-- ================= MODAL ================= -->

<div class="modal" id="modalImagen" onclick="cerrarImagen()">

    <span class="close">&times;</span>

    <img id="imagenGrande" src="" alt="Imagen ampliada">

</div>


<!-- ================= FOOTER ================= -->

<footer>

    <p>
        <strong>Uso adecuado del repelente para mosquitos</strong>
    </p>

    <p>
        Unidad Educativa de las Fuerzas Armadas
    </p>

    <p>
        Liceo Naval de Guayaquil «Cmdte. Rafael Andrade Lalama»
    </p>

    <p>
        1ro Delta · 22 de Septiembre de 2026
    </p>

    <p>
        Estudiante participante: Caiza Nicole
    </p>

</footer>


<script>

    function abrirImagen(imagen) {

        document.getElementById("imagenGrande").src = imagen;

        document.getElementById("modalImagen").style.display = "flex";

    }


    function cerrarImagen() {

        document.getElementById("modalImagen").style.display = "none";

    }


    document.addEventListener("keydown", function(event) {

        if (event.key === "Escape") {

            cerrarImagen();

        }

    });

</script>

</body>
</html>
