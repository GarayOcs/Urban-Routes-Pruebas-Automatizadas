
# 🚖 Urban Routes - Pruebas Automatizadas

## Descripción del Proyecto

Este proyecto contiene una suite de pruebas automatizadas para la aplicación web **Urban Routes**, la cual permite a los usuarios solicitar servicios de taxi de manera eficiente. Las pruebas verifican diversas funcionalidades, incluyendo:

- Configuración de direcciones de recogida y destino.
- Selección de tarifas específicas.
- Introducción de información de contacto y métodos de pago.
- Envío de mensajes al conductor.
- Solicitud de servicios adicionales, como mantas, pañuelos y helados.

## Tecnologías y Herramientas Utilizadas

- **Lenguaje**: Python 3.12.4
- **Automatización de Pruebas**: Selenium WebDriver
- **Gestión de Pruebas**: Pytest
- **Entorno de Desarrollo**: PyCharm Community Edition 2024.1.4

## Requisitos Previos

Antes de ejecutar las pruebas, asegúrate de tener instaladas las siguientes herramientas:

- **Python 3.12.4**: [Descargar](https://www.python.org/downloads/)
- **Google Chrome**: Última versión estable.
- **ChromeDriver**: Compatible con la versión de Chrome instalada. [Descargar](https://sites.google.com/chromium.org/driver/)

Instala las dependencias necesarias utilizando el siguiente comando:

```bash
pip install pytest selenium
```

## Estructura del Proyecto

- `main.py`: Contiene las clases y métodos que implementan las pruebas automatizadas.
- `data.py`: Almacena datos utilizados en las pruebas, como URLs, direcciones y números de teléfono.
- `README.md`: Documentación del proyecto (este archivo).

## Instrucciones para Ejecutar las Pruebas

1. **Configuración de ChromeDriver**:
   - Descarga ChromeDriver y colócalo en una carpeta accesible.
   - Asegúrate de agregar el directorio de ChromeDriver a tu variable de entorno `PATH` o colócalo en el mismo directorio del proyecto.

2. **Ejecución de las Pruebas**:
   - Clona el repositorio o descarga los archivos del proyecto.
   - Desde una terminal, navega hasta la carpeta que contiene el proyecto.
   - Ejecuta el siguiente comando para iniciar las pruebas:

     ```bash
     pytest main.py
     ```

   Asegúrate de que Google Chrome esté cerrado antes de iniciar las pruebas, ya que Selenium abrirá una nueva instancia del navegador para cada prueba.

3. **Verificación de los Resultados**:
   - Al finalizar la ejecución, recibirás un reporte en la terminal indicando el estado de cada prueba.
   - Analiza cualquier error detallado para solucionar posibles problemas en las pruebas o en la aplicación.

## Lista de Comprobación de Funcionalidades Probadas

1. Configurar la dirección de recogida y destino.
2. Seleccionar la tarifa "Comfort".
3. Rellenar el número de teléfono.
4. Agregar una tarjeta de crédito.
5. Escribir un mensaje para el conductor.
6. Solicitar una manta y pañuelos.
7. Pedir 2 helados.
8. Verificar la aparición del modal de búsqueda de taxi.
9. Esperar a que aparezca la información del conductor en el modal.

*Nota*: La última funcionalidad es opcional y puede ser eliminada si presenta inconvenientes.

## Entorno de Pruebas

- **Python**: 3.12.4
- **Pip**: 24.0
- **Sistema Operativo**: Windows 11
- **IDE**: PyCharm Community Edition 2024.1.4

*Nota*: Si encuentras problemas al ejecutar las pruebas desde el IDE, intenta correrlas desde la terminal con el siguiente comando:

```bash
pytest main.py
```
