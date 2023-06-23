### Imagen Wordpress 

- La siguiente imagen en Docker, nos permitirá tener un sitio Wordpress disponible y listo para su uso, esto es basado en la ultima version de Wordpress 2023, en una instancia EC2 amazon linux. 

##Como usar esta imagen

- Comenzamos por asignar el siguiente comando para poder obtener nuestra imagen: 

>>"docker pull douglas96/sitio:nombre_a_asignar"
>>>Recordar Que Debemos De Tener Instalado En Nuestra Maquina, el Lenguaje de "Docker"
- Esto descargará la imagen "douglas96/sitio" con la etiqueta asignada en tu sistema local.

###### Una vez que la imagen se haya descargado, puedes ejecutar un contenedor utilizando el siguiente comando.

>> docker run -d -p 80:80 douglas96/sitio:nombre_asignado

- Esto ejecutará un contenedor a partir de la imagen descargada y mapeará el puerto 80 del contenedor al puerto 80 del host. Ahora puedes acceder al sitio web en tu navegador visitando http://localhost.

- Podremos verificar con el siguiente comando las imagenes de nuestra maquina
>> docker images

### Tambien a modo de informacion, tenemos los archivos de configuracion de nuestro sitio, a disposicion. 
