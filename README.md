
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hotel JEJA</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }
        header {
            background: #2d6187;
            color: white;
            padding: 20px 10%;
            text-align: center;
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        nav {
            display: flex;
            justify-content: center;
            background: #1b4d66;
            padding: 10px;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
        }
        nav a:hover {
            text-decoration: underline;
        }
        section {
            padding: 20px 10%;
        }
        .btn-reserva {
            display: block;
            text-align: center;
            margin: 20px auto;
            padding: 10px 20px;
            background: #1b4d66;
            color: white;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
            width: 200px;
        }
        .btn-reserva:hover {
            background: #155366;
        }
        footer {
            text-align: center;
            background: #2d6187;
            color: white;
            padding: 10px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Bienvenidos al Hotel JEJA</h1>
        <p>Donde la comodidad y el lujo se encuentran</p>
    </header>
    <nav>
        <a href="#habitaciones">Habitaciones</a>
        <a href="#servicios">Servicios</a>
        <a href="#galeria">Galería</a>
        <a href="#reservas">Reservas</a>
        <a href="#contacto">Contacto</a>
    </nav>
    <section id="inicio">
        <h2>¡Reserva ahora tu estancia en el Hotel JEJA!</h2>
        <a href="reservar.html" class="btn-reserva">HAGA SU RESERVA</a>
    </section>
    <footer>
        <p>&copy; 2024 Hotel JEJA. Todos los derechos reservados.</p>
    </footer>
</body>
</html>
git checkout
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Haga su Reserva</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }
        header {
            background: #2d6187;
            color: white;
            padding: 20px;
            text-align: center;
        }
        form {
            max-width: 600px;
            margin: 20px auto;
            padding: 20px;
            border: 1px solid #ddd;
            border-radius: 5px;
            background: #f9f9f9;
        }
        fieldset {
            border: 1px solid #ddd;
            margin-bottom: 20px;
            padding: 15px;
        }
        legend {
            font-weight: bold;
            padding: 0 10px;
        }
        label {
            display: block;
            margin-bottom: 5px;
        }
        input, select, button {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        input[type="radio"], input[type="checkbox"] {
            width: auto;
            margin-right: 5px;
        }
        button {
            background: #1b4d66;
            color: white;
            border: none;
            cursor: pointer;
        }
        button:hover {
            background: #155366;
        }
        .link-back {
            text-align: center;
            display: block;
            margin-top: 20px;
            color: #2d6187;
            text-decoration: none;
            font-weight: bold;
        }
        .link-back:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <h1>Haga su reserva</h1>
    </header>
    <form action="procesareserva.php" method="GET">
        <fieldset>
            <legend>Datos Personales</legend>
            <label for="nombre">Nombre</label>
            <input type="text" id="nombre" name="nombre" maxlength="100" required autofocus>
            
            <label for="apellidos">Apellidos</label>
            <input type="text" id="apellidos" name="apellidos" maxlength="100" required>
            
            <label for="dni">DNI</label>
            <input type="text" id="dni" name="dni" maxlength="10" required placeholder="DNI con letra">
        </fieldset>
        <fieldset>
            <legend>Datos de su estancia</legend>
            <label>Habitación</label>
            <input type="radio" id="individual" name="habitacion" value="Individual">
            <label for="individual">Individual</label>
            <input type="radio" id="doble" name="habitacion" value="Doble">
            <label for="doble">Doble</label>
            <input type="radio" id="triple" name="habitacion" value="Triple">
            <label for="triple">Triple</label>

            <label for="personas">Número de personas</label>
            <select id="personas" name="personas">
                <option value="1">1</option>
                <option value="2">2</option>
                <option value="3">3</option>
            </select>
            
            <label for="mascotas">
                <input type="checkbox" id="mascotas" name="mascotas"> Llevo mascotas
            </label>
            
            <label for="fecha">Fecha de llegada</label>
            <input type="date" id="fecha" name="fecha">
            
            <label for="hora">Hora de llegada</label>
            <input type="time" id="hora" name="hora">
        </fieldset>
        <button type="submit">Enviar</button>
        <button type="reset">Reiniciar</button>
        <a href="index.html" class="link-back">Volver</a>
    </form>
</body>
</html>

