
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

