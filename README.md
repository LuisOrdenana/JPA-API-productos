# Principios de JPA (API de productos en Github)

A continuación, se detallan las partes principales del proyecto:

## Parte 1: Creación de la Entidad y el Repositorio

1. **Entidad `Producto`**:
   - Se creó una clase llamada `Producto` en el paquete `model`.
   - Esta clase representa los productos disponibles en la tienda.

![image](https://github.com/user-attachments/assets/c2a8147f-b6f7-4691-90ac-e2d9ba2a8dd2)


3. **Repositorio `ProductoRepository`**:
   - Se definió una interfaz llamada `ProductoRepository` en el paquete `repository`.
   - Esta interfaz proporciona métodos para acceder y manipular los datos de los productos en la base de datos.
  
![image](https://github.com/user-attachments/assets/f374b797-6494-464a-a640-bf293996946f)


## Parte 2: Implementación del Servicio

1. **Clase `ProductoService`**:
   - Se creó la clase `basededatos` en el paquete `service`.
   - Esta clase contiene la lógica de negocio relacionada con los productos.


![image](https://github.com/user-attachments/assets/74759e09-4826-4a30-a662-b084894b97d0)

## Parte 3: Controlador para la API

1. **Clase `ProductoController`**:
   - Se implementó la clase `ProductoController` en el paquete `controller`.
   - Esta clase define los endpoints REST para acceder a los productos.
  
![image](https://github.com/user-attachments/assets/3a9499b1-3526-44a3-9644-4e687346c680)


## Parte 4: Inicialización de la Base de Datos

1. **Carga de Datos de Prueba**:
   - Se configuró una clase especial para inicializar algunos objetos `Producto` al inicio de la aplicación.
   - Los datos de prueba incluyen productos como "Laptop", "Smartphone", "Monitor", "Teclado" y "Mouse".

![image](https://github.com/user-attachments/assets/5e702577-db77-46c4-ae38-3ac5036f1566)

## Parte 5: Ejecución y Pruebas

1. **Ejecución de la Aplicación**:
   - La aplicación se puede ejecutar desde el IDE o mediante el comando `mvn spring-boot:run`.

![image](https://github.com/user-attachments/assets/0d62bdd8-ebbc-49a7-9957-76a90e7077e6)

2. **Prueba de los Endpoints**:
   - Utiliza herramientas como Postman o cURL para probar los siguientes endpoints:
     - `GET /api/productos`
![image](https://github.com/user-attachments/assets/2b21bf34-5613-449f-ab8e-38421b2795ec)

     - `GET /api/productos/{id}`
![image](https://github.com/user-attachments/assets/8d67a2ba-8ad1-46fd-ba6b-d01049fed0b0)

     - `GET /api/productos/search?nombre={nombre}`
![image](https://github.com/user-attachments/assets/1af56f4b-8a37-434b-bfad-0a44a7bd203c)

     - `GET /api/productos/searchByPrecio?preciomin={preciomin}&preciomax={preciomax}`
![image](https://github.com/user-attachments/assets/c6dea882-cea7-44cd-bd2a-2605b9d0f6c5)


