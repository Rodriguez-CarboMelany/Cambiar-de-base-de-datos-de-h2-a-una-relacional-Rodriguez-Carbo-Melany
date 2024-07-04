# Cambiar-de-base-de-datos-de-h2-a-una-relacional-Rodriguez-Carbo-Melany
Este código es una aplicación Spring Boot para gestionar hoteles, la cual incluye controladores, servicios y repositorios para acceder a una base de datos PostgreSQL. A continuación, se describe cada parte del código:
![image](https://github.com/Rodriguez-CarboMelany/Cambiar-de-base-de-datos-de-h2-a-una-relacional-Rodriguez-Carbo-Melany/assets/174674789/901355ab-e554-4075-b861-623c32f28b3c)
Este controlador maneja las solicitudes HTTP. La anotación `@RestController` indica que esta clase es un controlador REST. El método search está mapeado a la ruta /hotels con `@GetMapping`, y devuelve una lista de hoteles obtenida del servicio HotelService.
![image](https://github.com/Rodriguez-CarboMelany/Cambiar-de-base-de-datos-de-h2-a-una-relacional-Rodriguez-Carbo-Melany/assets/174674789/64c901d1-2f9e-4250-a803-1668433b922a)
La clase Hotel es una entidad JPA que representa la tabla Hotel en la base de datos. Tiene campos `hotelId`, `hotelName`, y `hotelAddress` con sus respectivos getters y setters.
![image](https://github.com/Rodriguez-CarboMelany/Cambiar-de-base-de-datos-de-h2-a-una-relacional-Rodriguez-Carbo-Melany/assets/174674789/cde81b07-5afd-4129-b582-1effa937d2e2)
`HotelRepository` es un repositorio Spring Data que proporciona métodos CRUD para la entidad `Hotel`.
![image](https://github.com/Rodriguez-CarboMelany/Cambiar-de-base-de-datos-de-h2-a-una-relacional-Rodriguez-Carbo-Melany/assets/174674789/25bd451c-6cbd-4230-a4b3-f4fd42326985)
![image](https://github.com/Rodriguez-CarboMelany/Cambiar-de-base-de-datos-de-h2-a-una-relacional-Rodriguez-Carbo-Melany/assets/174674789/6553dd23-9949-475f-82a1-33fae4392b8b)
`HotelService` es una interfaz que define el método search. `HotelServiceImpl` es una implementación de esta interfaz que usa HotelRepository para buscar todos los hoteles en la base de datos.
`HotelsApplication` es la clase principal que inicia la aplicación Spring Boot.
![image](https://github.com/Rodriguez-CarboMelany/Cambiar-de-base-de-datos-de-h2-a-una-relacional-Rodriguez-Carbo-Melany/assets/174674789/55a74c7b-4ac7-48aa-bff0-0b6b69b16294)
Configuración (application.properties)
![image](https://github.com/Rodriguez-CarboMelany/Cambiar-de-base-de-datos-de-h2-a-una-relacional-Rodriguez-Carbo-Melany/assets/174674789/0949d1f4-1727-47b0-8ada-f72b6364bba1)
Ejecucion del programa 
![image](https://github.com/Rodriguez-CarboMelany/Cambiar-de-base-de-datos-de-h2-a-una-relacional-Rodriguez-Carbo-Melany/assets/174674789/edd536e0-3c92-44a5-8da0-cc413337c614)
![image](https://github.com/Rodriguez-CarboMelany/Cambiar-de-base-de-datos-de-h2-a-una-relacional-Rodriguez-Carbo-Melany/assets/174674789/28044426-24c5-42f4-ae75-0960b7907eef)
![image](https://github.com/Rodriguez-CarboMelany/Cambiar-de-base-de-datos-de-h2-a-una-relacional-Rodriguez-Carbo-Melany/assets/174674789/507ee7ef-ea91-435f-8707-a24b9f6a2705)
gracias 







