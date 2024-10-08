<html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WORKBENCHES</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            background-image: url("1600w-PriNvkfDEzU.jpg");
            background-size: cover; 
            background-repeat: no-repeat;
            background-attachment: fixed;
        }

        .container {
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.9); /* Fondo blanco con transparencia */
            border-radius: 10px; 
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            display: flex;
        }

        /* Estilos de las pestañas a la izquierda */
        .tabs {
            width: 200px;
            background-color: #333;
            display: flex;
            flex-direction: column;
            margin-right: 20px;
            border-radius: 10px;
        }

        .tabs button {
            background-color: #333;
            color: white;
            padding: 15px;
            text-align: left;
            border: none;
            outline: none;
            cursor: pointer;
            transition: background-color 0.3s ease;
            width: 100%;
            border-bottom: 1px solid #555;
            font-weight: bold;
        }

        .tabs button:hover {
            background-color: #555;
        }

        .tabs button.active {
            background-color: #005f7c;
            color: #fff;
        }

        .tab-content {
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.9);
            flex-grow: 1;
            display: none; /* Ocultar todo el contenido por defecto */
            border-radius: 10px;
            position: relative; /* Para posicionar el logo dentro de cada pestaña */
        }

        .tab-content.active {
            display: block; /* Mostrar solo el contenido activo */
        }

        /* Estilo del logo circular y pequeño */
        .header img,
        .logo {
            border-radius: 50%;
            width: 50px; /* Tamaño pequeño y consistente */
            height: 50px;
        }

        /* Estilo del logo en las pestañas (a la derecha en todas menos en la principal) */
        .logo-container {
            position: absolute;
            top: 20px;
            right: 20px; /* Logo alineado a la derecha */
        }

        /* Título centrado en la página principal */
        .main-tab h1 {
            text-align: center;
            color: #333;
            font-size: 24px;
            margin: 0;
        }

        h2 {
            color: #333;
            font-size: 20px;
            margin-bottom: 10px;
        }

        p {
            line-height: 1.6;
            color: #555;
            font-size: 16px;
        }

        ul {
            color: #555;
            font-size: 16px;
        }

        /* Botón de "Más información" */
        .more-info-btn {
            background-color: #333;
            color: white;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            text-align: center;
            margin-top: 20px;
        }

        .more-info-content {
            display: none;
            background-color: rgba(255, 255, 255, 0.9);
            padding: 20px;
            border-radius: 10px;
            margin-top: 10px;
        }

        /* Botón de "Más información" estilizado */
        .more-info-btn:hover {
            background-color: #555;
        }

        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 20px;
            width: 100%;
            margin-top: 20px;
        }

    </style>
</head>
<body>
    <div class="container">
        <!-- Pestañas a la izquierda -->
        <div class="tabs">
            <button class="tab-link active" onclick="openTab(event, 'quienes-somos')">¿Quiénes somos?</button>
            <button class="tab-link" onclick="openTab(event, 'vision')">Visión</button>
            <button class="tab-link" onclick="openTab(event, 'mision')">Misión</button>
            <button class="tab-link" onclick="openTab(event, 'imagen')">Imagen de la Empresa</button>
            <button class="tab-link" onclick="openTab(event, 'producto')">Producto</button>
        </div>

        <!-- Contenido de las pestañas -->
        <!-- Pestaña principal con logo a la izquierda y título centrado -->
        <div id="quienes-somos" class="tab-content active main-tab">
            <div class="header" style="display: flex; align-items: center;">
                <img src="file.jpg" alt="Logo" style="margin-right: 15px;"> 
                <h1>WORKBENCHES</h1>
            </div>
            <section>
                <h2>¿Quiénes somos?</h2>
                <p>Somos Metalforge Workbenches, dedicados a diseñar y fabricar bancos de trabajo para procesos de soldadura. Nuestro objetivo es abordar y resolver problemas recurrentes observados durante las prácticas y ejercicios de soldadura. Además, aspiramos a optimizar el tiempo y mejorar la productividad en estas actividades.</p>
            </section>
        </div>

        <!-- Otras pestañas solo con el logo alineado a la derecha -->
        <div id="vision" class="tab-content">
            <div class="logo-container">
                <img src="file.jpg" alt="Logo" class="logo"> 
            </div>
            <section>
                <h2>Visión</h2>
                <ul>
                    <li><strong>A corto plazo (4-5 años):</strong> Nos esforzamos por ganar reconocimiento en el mercado a nivel regional.</li>
                    <li><strong>A mediano plazo (6-9 años):</strong> Buscamos expandirnos a nivel nacional, consolidándonos como una marca reconocida y confiable en el sector.</li>
                    <li><strong>A largo plazo (10-20 años):</strong> Aspiramos a convertirnos en una marca de referencia a nivel continental, con una base sólida de clientes fieles y nuevos compradores constantes.</li>
                </ul>
            </section>
        </div>

        <div id="mision" class="tab-content">
            <div class="logo-container">
                <img src="file.jpg" alt="Logo" class="logo"> 
            </div>
            <section>
                <h2>Misión</h2>
                <p>Participamos en el mercado fabricando bancos de trabajo para procesos de soldadura con especificaciones técnicas y ergonómicas adaptadas a las necesidades de nuestros clientes, mejorando así la calidad de los trabajos de manufactura.</p>
            </section>
        </div>

        <div id="imagen" class="tab-content">
            <div class="logo-container">
                <img src="file.jpg" alt="Logo" class="logo"> 
            </div>
            <section>
                <h2>Imagen de la empresa</h2>
                <p>Nuestra imagen de empresa se basa en la excelencia, la innovación y la confiabilidad. Nos esforzamos por ofrecer productos de alta calidad que superen las expectativas de nuestros clientes. Ejemplo: <strong>"Metalforge Workbenches: Tu socio confiable en la fabricación de bancos de trabajo para soldadura."</strong></p>
            </section>
        </div>

        <div id="producto" class="tab-content">
            <div class="logo-container">
                <img src="file.jpg" alt="Logo" class="logo"> 
            </div>
            <section>
                <h2>Producto</h2>
                <img src="Referencia.png" alt="Producto">
            </section>
        </div>
    </div>

    <!-- Botón de "Más información" -->
    <div class="more-info-btn-container" style="text-align: center;">
        <button class="more-info-btn" onclick="toggleMoreInfo()">Más Información</button>
    </div>

    <div class="more-info-content" id="more-info-content">
        <p>Organización de Bogotá Distrito Capital</p>
    </div>

    <footer>
        <p>Contáctenos</p>
        <p>Organización de Bogotá Distrito Capital</p> 
    </footer>

      <script>
        function openTab(evt, tabId) {
            // Ocultar todos los contenidos de las pestañas
            var tabContent = document.getElementsByClassName("tab-content");
            for (var i = 0; i < tabContent.length; i++) {
                tabContent[i].style.display = "none";
                tabContent[i].classList.remove("active");
            }

            // Quitar la clase "active" de todos los botones
            var tabLinks = document.getElementsByClassName("tab-link");
            for (var i = 0; i < tabLinks.length; i++) {
                tabLinks[i].classList.remove("active");
            }

            // Mostrar el contenido actual y añadir la clase "active" al botón actual
            document.getElementById(tabId).style.display = "block";
            document.getElementById(tabId).classList.add("active");
            evt.currentTarget.classList.add("active");
        }

        function toggleMoreInfo() {
            var content = document.getElementById("more-info-content");
            if (content.style.display === "block") {
                content.style.display = "none";
            } else {
                content.style.display = "block";
            }
        }

        // Inicializar la pestaña principal visible al cargar la página
        document.getElementById("quienes-somos").style.display = "block";
    </script>
</body>
</html>
