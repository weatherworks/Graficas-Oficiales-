<html lang="es"><head></head><body>




    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Estación Meteorológica - Datos en Tiempo Real</title>
    <style>
        /* Reset de estilo */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Estilos para el cuerpo */
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            background: #eaf2f7; /* Fondo claro con un toque suave */
            color: #333;
        }

        /* Cabecera */
        header {
            background: linear-gradient(135deg, #ff4d4d, #4da6ff); /* Degradado rojo-azul */
            color: white;
            text-align: center;
            padding: 30px;
            border-radius: 0 0 20px 20px;
        }

        header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }

        header p {
            font-size: 1.2em;
        }

        /* Sección principal */
        main {
            padding: 20px;
            background-color: #f9f9f9; /* Fondo blanco */
        }

        .tables-section {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }

        /* Contenedores de tablas */
        .table-container {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            padding: 20px;
            width: 100%;
            max-width: 700px;
            margin-bottom: 20px;
            background: #f5f5f5; /* Fondo muy suave */
            border: 1px solid #ddd;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .table-container:hover {
            transform: scale(1.02);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }

        h2 {
            text-align: center;
            margin-bottom: 15px;
            font-size: 1.8em;
            color: #333;
            background: linear-gradient(135deg, #ff4d4d, #4da6ff);
            -webkit-background-clip: text;
            color: transparent;
            font-weight: bold;
        }

        /* Estilos de tabla */
        table {
            width: 100%;
            border-collapse: collapse;
            margin-bottom: 20px;
        }

        th,
        td {
            padding: 10px;
            text-align: center;
            border: 1px solid #ddd;
        }

        th {
            background-color: #4da6ff;
            color: white;
            font-weight: bold;
        }

        td {
            background-color: #f9f9f9;
        }

        /* Estilos para los iframes */
        iframe {
            display: block;
            margin: 0 auto;
            border: none;
            border-radius: 10px;
            max-width: 100%;
        }

        /* Pie de página */
        footer {
            text-align: center;
            padding: 20px;
            background-color: #333;
            color: white;
            margin-top: 30px;
            border-radius: 10px 10px 0 0;
        }

        footer p {
            font-size: 1.1em;
        }
    </style>



    <header>
        <h1>Estación Meteorológica</h1>
        <p>Datos en tiempo real desde ThingSpeak</p>
    </header>

    <main>
        <section class="tables-section">
            <!-- Tabla 1: Temperatura -->
            <div class="table-container">
                <h2>Temperatura</h2>
                <table>
                    <thead>
                        <tr>
                            <th>Temperatura (°C)</th>
                        </tr>
                    </thead>
                    <tbody>
                        <!-- Aquí puedes agregar los valores de temperatura que necesites -->
                    </tbody>
                </table>
                <iframe width="600" height="400" src="https://thingspeak.mathworks.com/channels/2699691/charts/1?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;title=Graficas+de+la+estaci%C3%B3n+meteorol%C3%B3gica&amp;type=line" frameborder="0"></iframe>
            </div>

            <!-- Tabla 2: Humedad -->
            <div class="table-container">
                <h2>Humedad</h2>
                <table>
                    <thead>
                        <tr>
                            <th>Humedad (%)</th>
                        </tr>
                    </thead>
                    <tbody>
                        <!-- Aquí puedes agregar los valores de humedad que necesites -->
                    </tbody>
                </table>
                <iframe width="600" height="400" src="https://thingspeak.mathworks.com/channels/2699691/charts/2?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;type=line&amp;update=15" frameborder="0"></iframe>
            </div>

            <!-- Tabla 3: Presión Atmosférica -->
            <div class="table-container">
                <h2>Presión Atmosférica</h2>
                <table>
                    <thead>
                        <tr>
                            <th>Presión (hPa)</th>
                        </tr>
                    </thead>
                    <tbody>
                        <!-- Aquí puedes agregar los valores de presión que necesites -->
                    </tbody>
                </table>
                <iframe width="600" height="400" src="https://thingspeak.mathworks.com/channels/2699691/charts/3?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;type=line&amp;update=15" frameborder="0"></iframe>
            </div>

            <!-- Tabla 4: Calidad del Aire -->
            <div class="table-container">
                <h2>Calidad del Aire</h2>
                <table>
                    <thead>
                        <tr>
                            <th>Calidad del Aire (AQI)</th>
                        </tr>
                    </thead>
                    <tbody>
                        <!-- Aquí puedes agregar los valores de calidad de aire que necesites -->
                    </tbody>
                </table>
                <iframe width="600" height="400" src="https://thingspeak.mathworks.com/channels/2699691/charts/5?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;type=line&amp;update=15" frameborder="0"></iframe>
            </div>

            <!-- Tabla 5: Radiación UV -->
            <div class="table-container">
                <h2>Radiación UV</h2>
                <table>
                    <thead>
                        <tr>
                            <th>Radiación UV</th>
                        </tr>
                    </thead>
                    <tbody>
                        <!-- Aquí puedes agregar los valores de radiación UV que necesites -->
                    </tbody>
                </table>
                <iframe width="600" height="400" src="https://thingspeak.mathworks.com/channels/2699691/charts/4?bgcolor=%23ffffff&amp;color=%23d62020&amp;dynamic=true&amp;results=60&amp;type=line&amp;update=15" frameborder="0"></iframe>
                <a href="[https://weatherworks.github.io/graficas-de-las-pagina-de-weatherwork/](https://weatherworks.github.io/Pagina-oficial-de-nuestra-empresa/)" class="highlighted-link">Volver a la pagina oficial</a>
            </div>
        </section>
    </main>

    <footer>
<p></p>
    </footer>        <p>&amp;co




</p></body></html>
