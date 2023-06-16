* Implementar Sitio Web en una Instancia EC2 (Amazon-Linux) y proporcionar el codigo en GitHub y en 	Docker.

1: Procedemos a crear una instancia EC2 en AWS
	- Al momento de crear nuestra instancia, debemos asegurarnos de permitir el trafico por HTTP/HTTPS
	- En caso contrario, deberemos de agregar en nuestro grupo de seguridad, la regla de entrada a HTTP/HTTPS a cualquier IP.
2: Actualizamos nuestra instancia y procedemos a instalar lo necesario.
	- #sudo yum upgrade
	- #yum install httpd.x86_64
	- #yum install git.x86_64
	- #yum install docker.x86_64
	- #sudo yum install -y mariadb105-server.x86_64
	- #yum install php8.1.x86_64
	- #yum install php8.1-mysqlnd.x86_64
3: Iniciamos los servicios instalados
	- #systemctl start httpd.services
	- #systemctl enable httpd.services
	- #systemctl start mariadb.services
	- #systemctl enable mariadb.services
	- #systemctl start php-fpm.service
	- #systemctl enable php-fpm.service
4: Procedemos a crear nuestro directorio en la siguiente ruta
	- #cd /var/www/html
	- #mkdir wordpress
5: Procedemos a descargar y exportar la ultima version de wordpress en el directorio creado
	- #wget https://wordpress.org/latest.tar.gz
	- #tar -xzf latest.tar.gz# 
