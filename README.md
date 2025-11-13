<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CIUDADANOS EN ACCION</title>
    <style>
        /* ------------------------------------- */
        /* 1. VARIABLES Y ESTILOS BASE */
        /* ------------------------------------- */
        :root {
            /* Colores de diseño: Fondo oscuro y contenido claro */
            --color-dark-bg: #1a1a1a; 
            --color-light-content: #f8f8f0; 
            /* Colores de acento */
            --color-red-cta: #d11c1c; 
            
            --color-text: #333333;
            --color-border: #999;
            --font-main: 'Arial', sans-serif;
            --width-content: 800px; /* Ancho fijo del contenedor principal */
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: var(--color-dark-bg);
            font-family: var(--font-main);
            color: var(--color-text);
            line-height: 1.5;
        }

        /* ------------------------------------- */
        /* 2. ESTRUCTURA CENTRALIZADA */
        /* ------------------------------------- */
        .page-container {
            width: 100%;
            display: flex;
            justify-content: center;
        }

        .main-content-wrapper {
            width: var(--width-content);
            background-color: var(--color-light-content);
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
            min-height: 200vh;
            position: relative;
        }
        
        /* ------------------------------------- */
        /* 3. BANNER SUPERIOR Y LOGO */
        /* ------------------------------------- */
        .header-banner {
            height: 300px;
            position: relative;
            /* REEMPLAZAR URL DE FONDO DEL BANNER AQUÍ */
            background-image: url('https://wallpapers.com/images/featured/fondods-marron-oscuro-k56c55z0r1wqm7i6.jpg'); 
            background-size: cover;
            background-position: center;
            border-bottom: 2px solid var(--color-border);
        }

        .logo-container {
            position: absolute;
            top: 50%; 
            left: 50%; 
            transform: translate(-50%, -50%); 
            width: 200px;
            height: 200px;
            border-radius: 50%;
            background-color: var(--color-light-content);
            border: 5px solid black;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 10px;
        }

        .logo-container img {
            width: 100%;
            height: 100%;
            object-fit: contain;
        }

        /* ------------------------------------- */
        /* 4. INTRODUCCIÓN Y CTA (UN SOLO BOTÓN ROJO) */
        /* ------------------------------------- */
        .introduction-section {
            /* Padding superior ajustado para compensar el menú eliminado */
            padding: 50px 40px 40px 40px; 
            text-align: left;
        }

        .introduction-section p {
            margin-bottom: 20px;
            font-size: 1.1em;
        }

        .cta-group {
            display: flex;
            align-items: center;
            gap: 20px;
            margin-bottom: 40px;
        }

        /* Estilo del Botón CTA (único) */
        .cta-button {
            padding: 12px 25px;
            background-color: var(--color-red-cta);
            color: white;
            text-decoration: none;
            font-weight: bold;
            text-transform: uppercase;
            border-radius: 4px;
            font-size: 1em;
            transition: all 0.2s ease;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
            border: none;
        }

        .cta-button:hover {
            background-color: #e53935; 
            box-shadow: 0 6px 8px rgba(0, 0, 0, 0.3);
            transform: translateY(-1px);
        }
        
        /* ------------------------------------- */
        /* 5. GALERÍA DE IMÁGENES (2 COLUMNAS) */
        /* ------------------------------------- */
        .gallery-section {
            padding: 0 40px 40px 40px;
            display: flex;
            gap: 20px;
        }

        .col-left { flex: 2; }
        .col-right {
            flex: 1; 
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .gallery-image {
            width: 100%;
            height: auto;
            border: 4px solid black; 
            display: block;
            object-fit: cover;
        }
        
        .image-large-container {
            height: 450px;
            overflow: hidden;
        }

        /* ------------------------------------- */
        /* 6. SECCIONES DE INFORMACIÓN ADICIONAL */
        /* ------------------------------------- */
        .additional-info-section {
            padding: 40px;
            border-top: 1px solid var(--color-border);
        }

        .info-block { margin-bottom: 30px; }

        .info-block h3 {
            border-bottom: 2px solid var(--color-border);
            padding-bottom: 5px;
            margin-bottom: 15px;
            font-size: 1.3em;
            text-transform: uppercase;
        }

        /* ------------------------------------- */
        /* 7. BARRA LATERAL FIJA (DERECHA) */
        /* ------------------------------------- */
        .fixed-sidebar {
            position: fixed;
            top: 0;
            right: 0;
            width: 250px;
            height: 100%;
            background-color: var(--color-dark-bg);
            color: white;
            padding-top: 10px;
            z-index: 100;
        }

        .sidebar-item {
            display: flex;
            align-items: center;
            padding: 10px 15px;
            margin-bottom: 5px;
            cursor: pointer;
            transition: background-color 0.2s;
        }

        .sidebar-item:hover {
            background-color: rgba(255, 255, 255, 0.1);
        }

        .sidebar-item-icon {
            margin-right: 10px;
            font-size: 1.2em;
        }
        
        @media (max-width: 1050px) {
            .fixed-sidebar { display: none; }
        }

    </style>
</head>
<body>

    <div class="page-container">
        <div class="main-content-wrapper">
            
            <!-- 1. BANNER Y LOGO SUPERIOR -->
            <div class="header-banner">
                <div class="logo-container">
                    <!-- REEMPLAZAR URL DE IMAGEN DEL LOGO AQUÍ -->
                    <img src="https://cdn-icons-png.flaticon.com/512/9746/9746687.png" alt="Logo de la página">
                </div>
            </div>

            <!-- 2. INTRODUCCIÓN Y BOTÓN CTA (UN SOLO BOTÓN ROJO) -->
            <div class="introduction-section">
                <!-- REEMPLAZAR TEXTO DE DESCRIPCIÓN PRINCIPAL AQUÍ -->
                <p>
                    <center><strong>CIUDADANOS EN ACCION</strong></center>
                    <p>
                        El consumo de drogas se refiere al uso de sustancias que alteran el funcionamiento del cuerpo y la mente. Estas sustancias pueden cambiar cómo pensamos, sentimos o actuamos, y algunas generan dependencia, lo que significa que la persona siente la necesidad de consumirlas continuamente.
                </p>

                <div class="cta-group">
                    <!-- REEMPLAZAR TEXTO DEL BOTÓN ROJO DE ACCIÓN AQUÍ -->
                    <a href="#" class="cta-button">JUNTOS CONTRA LAS DROGAS</a>
                    
                    <!-- REEMPLAZAR TEXTO ADICIONAL JUNTO AL BOTÓN AQUÍ -->
                    <span>
                       
                    "La droga te roba el futuro. Hoy es el día para decir 'No' y tomar el control de tu vida".
                    </span>
                </div>
            </div>
            
            <!-- 3. GALERÍA DE IMÁGENES (2 COLUMNAS) -->
            <div class="gallery-section">
                <div class="col-left">
                    <!-- REEMPLAZAR URL DE IMAGEN GALERÍA GRANDE AQUÍ -->
                    <div class="image-large-container">
                        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTPWZZI1dvi0FvNjWRNhiyYTd9KD62aXN1LAg&s" alt="Captura de pantalla principal" class="gallery-image">
                    </div>
                </div>
                
                <div class="col-right">
                    <!-- REEMPLAZAR URL DE IMAGEN PEQUEÑA 1 AQUÍ -->
                    <img src="https://controllab.com/wp-content/uploads/Drogas-de-abuso-1.jpg" alt="Captura de pantalla secundaria 1" class="gallery-image">

                    <!-- REEMPLAZAR URL DE IMAGEN PEQUEÑA 2 AQUÍ -->
                    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQXec6KOVLXModPC34356yQCGqePGVJZ3Q2fg&s" alt="Captura de pantalla secundaria 2" class="gallery-image">
                    
                    <!-- REEMPLAZAR URL DE IMAGEN PEQUEÑA 3 AQUÍ -->
                    <img src="https://cuidadores.unir.net/images/post/drogas-jovenes.jpg" alt="Captura de pantalla secundaria 3" class="gallery-image">
                </div>
            </div>

            <!-- 4. SECCIÓN DE INFORMACIÓN ADICIONAL 1 -->
            <div class="additional-info-section">
                <div class="info-block">
                    <!-- REEMPLAZAR TÍTULO 1 AQUÍ -->
                    <strong><h3>El Alto Precio de la Criminalidad:</h3></strong>
                    <!-- REEMPLAZAR CONTENIDO 1 AQUÍ -->
                    <p>
  Comprar drogas no es un acto privado; es un soporte directo a las redes de crimen organizado y la violencia. . Cada dosis financia la corrupción, la inseguridad y la destrucción del tejido social. Combatir las drogas es también luchar por una comunidad más segura y en paz.
                    </p>
                </div>
                
                <!-- REEMPLAZAR URL DE IMAGEN/GRÁFICO ADICIONAL 1 AQUÍ -->
                <img src="https://img.freepik.com/fotos-premium/adiccion-al-alcohol-drogas-hombre-cigarrillos-humeantes-whisky-pastillas-mesa-textura-gris_495423-80510.jpg?semt=ais_hybrid&w=740&q=80" alt="Gráfico o imagen secundaria" style="width: 100%; height: auto; margin-bottom: 30px; border: 1px solid var(--color-border);">

                <div class="info-block">
                    <!-- REEMPLAZAR TÍTULO 2 AQUÍ -->
                    <h3>Riesgos Clave: Las drogas comprometen tu vida en múltiples aspectos:</h3>
                    <!-- REEMPLAZAR CONTENIDO 2 (Lista) AQUÍ -->
                    <ul>
                        <li>Problemas legales.</li>
                        <li>Aislamiento social.</li>
                        <li>Deterioro de la salud física.</li>
                    </ul>
                </div>
            </div>
            
            <!-- 5. SECCIÓN DE INFORMACIÓN ADICIONAL 2 -->
            <div class="additional-info-section">
                 <div class="info-block">
                    <!-- REEMPLAZAR TÍTULO 3 AQUÍ -->
                   <strong> <h3>EL ENGAÑO DE LA FUGA</h3></strong>
                    <!-- REEMPLAZAR CONTENIDO 3 AQUÍ -->
                    <p>
                         Aunque prometen un escape temporal de los problemas o el dolor, las drogas son una ilusión. Solo crean una dependencia que agrava los desafíos preexistentes, convirtiendo la búsqueda de alivio en una cadena de sufrimiento continuo.
                    </p>
                </div>
                <!-- REEMPLAZAR URL DE IMAGEN/GRÁFICO ADICIONAL 2 AQUÍ -->
                <img src="https://i0.wp.com/universal.org.mx/wp-content/uploads/2021/08/art-origen-de-las-adicciones.jpg?fit=860%2C525&ssl=1" alt="Gráfico o imagen secundaria 2" style="width: 100%; height: auto; margin-bottom: 30px; border: 1px solid var(--color-border);">

                 <div class="info-block">
                    <!-- REEMPLAZAR TÍTULO 4 AQUÍ -->
                   <strong> <h3>  La Recuperación es Posible:</h3></strong>
                    <!-- REEMPLAZAR CONTENIDO 4 AQUÍ -->
                    <p>
                       Romper el ciclo es difícil, pero totalmente viable. Millones de personas demuestran que la ayuda profesional, el apoyo de la comunidad y la perseverancia reconstruyen la vida . Busca apoyo; Nunca es demasiado tarde para empezar de nuevo.
                    </p>
                </div>
            </div>
            
        </div>
    </div>

</body>
</html>
