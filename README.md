<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hoja de Vida - Leydi Sarmiento</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #ffd6eb;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        .container {
            max-width: 800px;
            margin: auto;
            padding: 20px;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            margin-top: 50px;
        }
        .profile-pic {
            width: 150px;
            height: 150px;
            object-fit: cover;
            border-radius: 10px;
            border: 3px solid #ff0080;
        }
        .buttons {
            margin-top: 20px;
        }
        .buttons button {
            background-color: #ff0080;
            color: white;
            border: none;
            padding: 10px 15px;
            margin: 5px;
            cursor: pointer;
            border-radius: 5px;
        }
        .buttons button:hover {
            background-color: #e60073;
        }
        .content {
            display: none;
            margin-top: 20px;
            padding: 10px;
            border: 1px solid #ff0080;
            border-radius: 5px;
            background-color: #ffe6f2;
        }
        .active {
            display: block;
        }
        .pdf-container {
            margin-top: 20px;
        }
        .pdf-container iframe {
            width: 100%;
            height: 500px;
            border: none;
        }
        .pdf-container a {
            display: block;
            margin-top: 10px;
            background-color: #ff0080;
            color: white;
            padding: 10px;
            border-radius: 5px;
            text-decoration: none;
        }
        .pdf-container a:hover {
            background-color: #e60073;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Hoja de Vida - Leydi Sarmiento</h1>
        <img src="LEIDY.jfif" alt="Foto de Perfil" class="profile-pic">
        <div class="buttons">
            <button onclick="showContent('perfil')">Perfil</button>
            <button onclick="showContent('experiencia')">Experiencia</button>
            <button onclick="showContent('educacion')">Educación</button>
            <button onclick="showContent('gustos')">Gustos</button>
        </div>
        <div id="perfil" class="content active">
            <h2>Perfil</h2>
            <p>Soy una persona proactiva y creativa. Me gusta trabajar en equipo y dar soluciones para optimizar tareas. Estoy capacitada en gestión de proyectos y me apasiona la tecnología.</p>
        </div>
        <div id="experiencia" class="content">
            <h2>Experiencia</h2>
            <p>He trabajado en el área de soporte técnico y desarrollo de software, asegurando el correcto funcionamiento de los sistemas y optimizando procesos mediante herramientas digitales.</p>
        </div>
        <div id="educacion" class="content">
            <h2>Educación</h2>
            <p>Estudiante de Desarrollo de Software con certificación en Técnica en Sistemas por el SENA.</p>
        </div>
        <div id="gustos" class="content">
            <h2>Gustos</h2>
            <p>Me encanta la tecnología, escuchar música y bailar en mi tiempo libre.</p>
        </div>

        <div class="pdf-container">
            <h2>Mi Hoja de Vida</h2>
            <iframe src="Hoja de vida.pdf"></iframe>
            <a href="" download>Descargar Hoja de Vida (PDF)</a>
        </div>
    </div>
    <script>
        function showContent(section) {
            document.querySelectorAll('.content').forEach(content => {
                content.classList.remove('active');
            });
            document.getElementById(section).classList.add('active');
        }
    </script>
</body>
</html>
