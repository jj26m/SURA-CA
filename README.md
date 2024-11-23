# SURA-CA
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GRUPO SURA</title>
    <style>
        /* Estilos básicos */
        body {
            font-family: Arial, sans-serif;
            background-color: #f5f5f5;
            color: #333;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #ffffff;
            text-align: center;
            padding: 20px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        header h1 {
            color: #007bff;
            font-size: 2.5rem;
            margin: 0;
        }

        header img {
            max-width: 300px;
            margin-top: 10px;
        }

        header p {
            font-size: 1.1rem;
            color: #007bff;
            margin: 5px 0 0;
        }

        .creator {
            position: absolute;
            top: 10px;
            right: 20px;
            text-align: center;
        }

        .creator img {
            width: 40px;
            border-radius: 50%;
        }

        .creator p {
            font-size: 0.9rem;
            margin-top: 5px;
        }

        .menu {
            display: flex;
            justify-content: center;
            margin: 20px;
        }

        .menu button {
            background-color: #007bff;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            margin: 0 10px;
            cursor: pointer;
            font-size: 1.2em;
        }

        .menu button:hover {
            background-color: #0056b3;
        }

        .form-section {
            display: none;
            margin: 20px;
            padding: 20px;
            background-color: white;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }

        form input, form select {
            margin: 10px 0;
            padding: 10px;
            width: 100%;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        .submit-btn {
            background-color: #007bff;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .submit-btn:hover {
            background-color: #0056b3;
        }

        footer {
            text-align: center;
            padding: 20px;
            background-color: #ffffff;
            border-top: 1px solid #ddd;
            margin-top: 20px;
            color: #555;
        }
    </style>
</head>
<body>
    <header>
        <h1>GRUPO SURA</h1>
        <img src="https://via.placeholder.com/300x100?text=GRUPO+SURA" alt="Grupo Sura">
        <p>NUESTRO MEJOR ACTIVO, LA GENTE UNA EMPRESA SEGURA Y SALUDABLE</p>
    </header>

    <div class="creator">
        <img src="https://via.placeholder.com/50x50" alt="Creador">
        <p>CREADOR: JJ26M</p>
    </div>

    <div class="menu">
        <button onclick="showSection('seguros')">Seguros</button>
        <button onclick="showSection('trabajos')">Ofertas de Trabajo</button>
        <button onclick="showSection('citas')">Citas Médicas</button>
    </div>

    <!-- Sección de Seguros -->
    <div id="seguros" class="form-section">
        <h2>Seguros</h2>
        <form id="segurosForm">
            <select name="tipo" required>
                <option value="" disabled selected>Tipo de Seguro</option>
                <option value="Médico">Médico</option>
                <option value="Propiedades">Propiedades</option>
            </select>
            <input type="text" name="user" placeholder="Usuario" required>
            <input type="text" name="nombre" placeholder="Nombre y Apellidos" required>
            <input type="text" name="sujeto" placeholder="Sujeto del Seguro" required>
            <input type="number" name="duracion" placeholder="Duración (meses)" required>
            <button type="submit" class="submit-btn">Enviar</button>
        </form>
    </div>

    <!-- Sección de Trabajos -->
    <div id="trabajos" class="form-section">
        <h2>Ofertas de Trabajo</h2>
        <form id="trabajosForm">
            <select name="puesto" required>
                <option value="" disabled selected>Selecciona un Puesto</option>
                <option value="Paramédico">Paramédico</option>
                <option value="Enfermería">Enfermería</option>
                <option value="Médico">Médico</option>
                <option value="Cirujano">Cirujano</option>
            </select>
            <input type="text" name="user" placeholder="Usuario" required>
            <input type="text" name="nombre" placeholder="Nombre y Apellidos" required>
            <input type="number" name="edad" placeholder="Edad" required>
            <input type="text" name="experiencias" placeholder="Experiencias" required>
            <button type="submit" class="submit-btn">Enviar</button>
        </form>
    </div>

    <!-- Sección de Citas Médicas -->
    <div id="citas" class="form-section">
        <h2>Citas Médicas</h2>
        <form id="citasForm">
            <input type="text" name="user" placeholder="Usuario" required>
            <input type="text" name="nombre" placeholder="Nombre y Apellidos" required>
            <input type="number" name="edad" placeholder="Edad" required>
            <input type="text" name="consulta" placeholder="Tipo de Consulta" required>
            <input type="datetime-local" name="fecha" required>
            <button type="submit" class="submit-btn">Enviar</button>
        </form>
    </div>

    <footer>
        &copy; 2024 GRUPO SURA. Todos los derechos reservados.
    </footer>

    <script>
        function showSection(sectionId) {
            const sections = document.querySelectorAll('.form-section');
            sections.forEach(section => section.style.display = 'none');
            document.getElementById(sectionId).style.display = 'block';
        }
    </script>
</body>
</html>
