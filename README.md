# Proyecto 01, Web Service.

Repositorio para el Proyecto 01 de Modelado y Programación.

Prof. José Galaviz Casas.

Este proyecto consiste en una página web que consulta en tiempo real el clima de destinos de vuelo, ya sea introduciendo directamente una ciudad o mediante el código de un ticket de vuelo que parte o llega al AICM. 

## Integrantes

+ Oscar Yahir Hernandez Garcia // **Rol: Project Manager y desarrollador Front-End** 
+ Said Apis Lorenzana // **Rol: Desarrollador Back-End**
+ Gerardo Gael Sandoval Sandoval // **Rol: Beta-Tester y desarrollador de pruebas unitarias** 

## Descripción

Este proyecto está desarrollado utilizando Python, JavaScript, HTML y CSS. Proporciona una implementación de un servicio web utilizando Flask, entre otras herramientas.

## Instalación

Para configurar el entorno de desarrollo, sigue estos pasos:

1. **Clona el repositorio:**

   ```Bash
   git clone https://github.com/Yahir-Hernandez/Proyecto01_Web_Service.git
   cd Proyecto01_Web_Service/weather_app
   ```

## Antes de Ejecutar

Una vez instado el proyecto, es necesario hacer algunos ajustes. 

Para funcionar correctamente, nuestra página necesita de una key *Hourly Forecast 4 days* de [OpenWeatherMap](https://openweathermap.org/api) y una key personal de [AviationStack](https://aviationstack.com/). 
Ambas pueden obtenerse gratuitamente haciendo un registro corto. En el caso de OpenWeatherMap, también es necesesario presentar una credencial de estudiante. 

Una vez obtenidas e instalado el proyecto, visita la ruta:

```bash
<tu_ruta_a_este_proyecto>/weather_app/utils/.env
```
Y modifica los apartados WEATHER_KEY y FLIGHT_KEY para que coincidan con tus claves de OpenWeatherMap y AviationStack, respectivamente.

## Ejectutar el Proyecto

Una vez completados los pasos anteriores:

1. **Ejecuta el modulo install.py:**

   En la carpeta weather_app/ del proyecto, encontrarás un módulo de Python llamado install.py. Este módulo crea un entorno virtual de Python e instalara todos los paquetes necesarios para ejecutar el proyecto.
   
   Ejecuta el siguiente comando para configurar el entorno:
   
   ```bash
   python3 install.py
   ```
   
   Esto creará un entorno virtual y instalará los siguientes paquetes requeridos:
   
   * beautifulsoup4==4.12.3
   * blinker==1.8.2
   * certifi==2024.8.30
   * chardet==3.0.4
   * charset-normalizer==3.3.2
   * click==8.1.7
   * deep-translator==1.11.4
   * Flask==3.0.3
   * fuzzywuzzy==0.18.0
   * googletrans==4.0.0rc1
   * h11==0.9.0
   * h2==3.2.0
   * hpack==3.0.0
   * hstspreload==2024.9.1
   * httpcore==0.9.1
   * httpx==0.13.3
   * hyperframe==5.2.0
   * idna==2.10
   * iniconfig==2.0.0
   * itsdangerous==2.2.0
   * Jinja2==3.1.4
   * Levenshtein==0.25.1
   * MarkupSafe==2.1.5
   * numpy==2.1.0
   * packaging==24.1
   * pandas==2.2.2
   * pluggy==1.5.0
   * pytest==8.3.2
   * python-dateutil==2.9.0.post0
   * python-dotenv==1.0.1
   * pytz==2024.1
   * rapidfuzz==3.9.6
   * requests==2.32.3
   * rfc3986==1.5.0
   * six==1.16.0
   * sniffio==1.3.1
   * soupsieve==2.6
   * tzdata==2024.1
   * urllib3==2.2.2
   * Werkzeug==3.0.4

   Después de instalar los paquetes, se ejecutará flask y se creará el link a la página Web.

##  **Prueba de búsqueda por tickets**

Por último, en nuestra página puedes consultar climas asociados al origen y al destino de vuelos completamente reales. Para probar este apartado, sugerimos que una vez ejecutado el proyecto, visites la ruta:

```bash
<tu_ruta_a_este_proyecto>/weather_app/utils/cache/
```
Y consultes el archivo:

```bash
ejemplo_tickets.txt
```
Que tendrá escritos algunos tickets recuperados en tiempo real desde la página oficial del [Aereopuerto Internacional de la Ciudad de México](https://www.aicm.com.mx/pasajeros/vuelos
). Otra opción para probar este apartado es copiar y pegar algún ticket de vuelo (localizados en la columna vuelos) desde la página antes mencionada, e ingresarlo en nuestro proyecto.


