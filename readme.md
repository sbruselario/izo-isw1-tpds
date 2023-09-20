
# IZO - Ingeniería de Software 1

- Identifique los requerimientos.
- Confeccione el diccionario de datos.
- Identifique las reglas de negocio.
- Realice el caso de uso.
- Construya el diagrama entidad-relación y el diagrama de clases.
- Realice el diagrama de secuencia.

> Una cámara de videocontrol vial, mide la velocidad con la que los autos pasan por una calle. En la ciudad, se cuentan con *n* cantidad de cámaras. Cada cámara, detecta automáticamente al vehículo cuando pasa y envía a nuestro sistema los siguientes datos: fecha y hora, id de la cámara, patente y velocidad. El paso de cada vehículo deberá registrarse en el sistema.
Cada cámara tiene un id, una descripción, coordenadas x e y de su ubicación, dirección IP y modelo de la cámara.
El sistema debe funcionar 24/7.

Cuando el sistema recibe los datos de un vehículo que pasó, el sistema realiza distintas acciones según la velocidad:
> - si la velocidad es mayor a 70km/h:  
>   - el sistema envía los datos a una API que se encargará de guardarlos en una base de datos
>   - el sistema envía un correo con los datos que envió la cámara a la cuenta "avisos@ciudad"
> - si la velocidad es mayor a 100km/h: 
>   - el sistema envía los datos a una API que se encargará de guardarlos en una base de datos
>   - el sistema envía un correo con los datos que envió la cámara a la cuenta "alertas@ciudad"
>   - el sistema envía, 3 veces, los datos recibidos por la cámara a una impresora para que sean impresos
>   

