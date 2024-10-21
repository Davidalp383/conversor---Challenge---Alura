# conversorApp --- Challenge --- Alura

---

# Conversor de Moneda - Aplicación Java MVC

Este proyecto es una aplicación de consola diseñada para facilitar la conversión de monedas utilizando tasas de cambio en tiempo real extraídas de una API externa. Implementada bajo el patrón de diseño *Modelo-Vista-Controlador (MVC)*, esta herramienta asegura una organización clara del código y una fácil escalabilidad y mantenimiento.

## Resumen del Proyecto

El *Conversor de Moneda* es una aplicación sencilla y efectiva que permite a los usuarios realizar conversiones entre varias monedas, aprovechando las tasas de cambio actualizadas en tiempo real a través de la *API de ExchangeRate*. La aplicación proporciona una interfaz de usuario en consola y permite las conversiones entre las siguientes monedas:

- Dólar estadounidense (USD) ⇆ Peso argentino (ARS)
- Dólar estadounidense (USD) ⇆ Real brasileño (BRL)
- Dólar estadounidense (USD) ⇆ Peso colombiano (COP)

Desarrollado en *Java* sin el uso de frameworks adicionales, el programa utiliza la biblioteca *HttpClient* para realizar solicitudes a la API y *Gson* para manejar la respuesta JSON.

## Características Principales

- Conversión de monedas en tiempo real.
- Acceso a tasas de cambio actualizadas desde la API.
- Menú interactivo en consola, intuitivo y fácil de navegar.
- Gestión eficiente de errores y excepciones.
- Estructura basada en el patrón *Modelo-Vista-Controlador (MVC)*.

## Estructura del Proyecto

El proyecto está organizado en torno al patrón MVC, con la siguiente estructura de paquetes:

- *model*: Lógica de negocio y comunicación con la API de tasas de cambio.
- *view*: Interfaz de usuario para la interacción con el usuario (consola).
- *controller*: Coordina las interacciones entre el modelo y la vista, gestionando el flujo de la aplicación.
- *exceptions*: Excepciones personalizadas para el manejo específico de errores.

## Tecnologías Utilizadas

- *Java*: Lenguaje principal del proyecto.
- *HttpClient*: Para realizar solicitudes HTTP a la API.
- *Gson*: Para procesar respuestas en formato JSON.
- *MVC Pattern*: Diseño estructural de la aplicación.

## Guía de Instalación

1. Clona el repositorio:
   bash
   git clone https://github.com/tu-repositorio/conversor-moneda-java.git
   

2. Abre el proyecto en tu entorno de desarrollo preferido.

3. Asegúrate de incluir la biblioteca Gson en tu proyecto. Si no la tienes, descárgala o agrega la siguiente dependencia de Maven:
   xml
   <dependency>
       <groupId>com.google.code.gson</groupId>
       <artifactId>gson</artifactId>
       <version>2.8.9</version>
   </dependency>
   

4. Ejecuta el archivo ConversorApp.java para comenzar a usar la aplicación.

## Uso de la Aplicación

1. Al iniciar la aplicación, se presentará un menú con varias opciones de conversión.
2. Selecciona la opción correspondiente a la conversión que deseas realizar.
3. La aplicación recuperará las tasas de cambio actuales desde la API y mostrará el resultado de la conversión.
4. Puedes realizar múltiples conversiones hasta que decidas salir.

## API Utilizada

Este proyecto se apoya en la *API ExchangeRate* para acceder a tasas de cambio en tiempo real. El endpoint principal utilizado es:

- *Endpoint*: https://v6.exchangerate-api.com/v6/apiKey/latest/{moneda_base}

Por ejemplo, para obtener la tasa de cambio del dólar estadounidense (USD):

https://v6.exchangerate-api.com/v6/apiKey/latest/USD

## Licencia

Este proyecto está bajo la Licencia MIT. Para más detalles, consulta el archivo LICENSE.

---
