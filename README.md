# Portafolio.DiegoAlvarado.io
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portafolio de Diego Alvarado González</title>
    <style>
        /* Estilos generales */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }

        /* Encabezado */
        header {
            background-color: #333;
            color: #fff;
            padding: 20px;
            text-align: center;
        }

        header h1 {
            margin: 0;
            font-size: 1.5em;
        }

        /* Navegación */
        nav {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            background-color: #444;
            padding: 10px;
        }

        nav a {
            color: #fff;
            padding: 10px 20px;
            text-decoration: none;
        }

        nav a:hover {
            background-color: #666;
        }

        /* Secciones */
        section {
            padding: 20px;
            margin: 20px;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }

        /* Footer */
        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 10px;
            width: 100%;
        }

        /* Estilos de video */
        video {
            width: 100%;
            height: auto;
            max-width: 500px;
        }

        /* Media queries para pantallas móviles */
        @media (max-width: 768px) {
            header, nav, footer {
                text-align: center;
            }

            nav a {
                padding: 8px 10px;
                font-size: 0.9em;
            }

            section {
                margin: 10px;
                padding: 15px;
            }

            header h1 {
                font-size: 1.2em;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>Portafolio de Diego Alvarado González</h1>
    </header>

    <nav>
        <a href="#acerca-de-mi">Acerca de Mí</a>
        <a href="#cv">CV</a>
        <a href="#portfolio">Portafolio</a>
        <a href="#demo-reel">Demo Réel</a>
        <a href="#video-presentacion">Vídeo Presentación</a>
        <a href="#contacto">Contacto</a>
    </nav>

    <main>
        <!-- Sección Acerca de Mí -->
        <section id="acerca-de-mi">
            <h2>Acerca de Mí</h2>
            <p>Bienvenido a mi portafolio personal. Soy Diego Alvarado González, un apasionado del diseño, animación y arte digital.</p>
        </section>

        <!-- Sección CV -->
        <section id="cv">
            <h2>CV</h2>
            <p>Aquí puedes ver mi trayectoria profesional y académica.</p>
         <a href="Copia de curriculum-2.pdf.pdf">Descargar CV</a></section>

      <!-- Sección Portafolio -->
<section id="portfolio">
    <h2>Portafolio</h2>
    <p>Aquí podrás ver algunos de mis trabajos de modelado 3D, animación y edición de video.</p>
    <p>Escanea el código QR para ver más ejemplos de mis proyectos:</p>
    <img src="QR.png" alt="Código QR para acceder al portafolio" class="qr-code">
</section>




       <!-- Sección Demo Réel -->
<section id="demo-reel">
    <h2>Demo Réel</h2>
    <p>Mira mi Demo Réel para ver un resumen de mis habilidades y proyectos.</p>
    
    <!-- Botón para seleccionar video -->
    <input type="file" id="videoUploader" accept="video/mp4,video/x-m4v,video/*">
    
    <!-- Video para previsualización -->
    <video id="demoReelVideo" controls>
        <source src="file:///C|/Users/Diego/OneDrive - Laureate Mexico/Desktop/Pagina_web/tu_video_demo_reel.mp4" type="video/mp4">
        Tu navegador no soporta este video.
    </video>
</section>

<script>
    // JavaScript para actualizar el video con el archivo seleccionado
    document.getElementById('videoUploader').addEventListener('change', function(event) {
        const file = event.target.files[0];
        const video = document.getElementById('demoReelVideo');
        
        if (file) {
            const videoURL = URL.createObjectURL(file);
            video.src = videoURL;
            video.load();
            video.play();
        }
    });
</script>


        <!-- Sección Vídeo Presentación -->
<section id="video-presentacion">
    <h2>Vídeo Presentación</h2>
    <p>Conoce más sobre mí a través de mi video de presentación.</p>
    
    <!-- Botón para seleccionar video -->
    <input type="file" id="videoUploaderPresentacion" accept="video/mp4,video/x-m4v,video/*">
    
    <!-- Video para previsualización -->
    <video id="videoPresentacion" controls>
        <source src="file:///C|/Users/Diego/OneDrive - Laureate Mexico/Desktop/Pagina_web/tu_video_presentacion.mp4" type="video/mp4">
        Tu navegador no soporta este video.
    </video>
</section>

<script>
    // JavaScript para actualizar el video con el archivo seleccionado
    document.getElementById('videoUploaderPresentacion').addEventListener('change', function(event) {
        const file = event.target.files[0];
        const video = document.getElementById('videoPresentacion');
        
        if (file) {
            const videoURL = URL.createObjectURL(file);
            video.src = videoURL;
            video.load();
            video.play();
        }
    });
</script>

        <!-- Sección Contacto -->
        <section id="contacto">
            <h2>Contacto</h2>
            <p>Si deseas contactarme, puedes hacerlo a través de mis redes sociales o enviándome un mensaje.</p>
            <ul>
                <li>Email: <a href="mailto:moldeado181@gmail.com">moldeado181@gmail.com</a></li>
                <li>LinkedIn: <a href="https://www.linkedin.com/in/diego-alvarado-72b0922ab?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank">Mi LinkedIn</a></li>
            </ul>
        </section>
    </main>

    <footer>
      <p>&copy; 2024 Diego Alvarado González. Todos los derechos reservados.</p>
</footer>

</body>
</html>
