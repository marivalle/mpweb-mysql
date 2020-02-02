# MPWEB Bases de Datos - MySQL 
Bienvenidos a la imagen de MySQL para a la asignatura de Bases de Datos del master [Máster en Programación Web Online (MPWEB)](https://www.salleurl.edu/es/estudios/master-en-programacion-web-online)

Para arrancar el MySQL y empezar a utilizar la imagen de docker realizar lo siguiente:

*Requisito previo: tener instalado docker*

1) Clonar el repositorio
```bash
git clone https://github.com/marivalle/mpweb-mysql.git
```
2) Arrancar la imagen de docker
```bash
cd mpweb-mysql
## En modo stdout
docker-compose up
## En modo silencioso
docker-compose up -d
```
3) Una vez haya arrancado podemos acceder al MySQL utilizando el siguiente comando:
```
docker exec -ti mpweb-mysql_db_1 mysql -u user -ptest 
```
y si queremos acceder como root
```
docker exec -ti mpweb-mysql_db_1 mysql -u root -proot
```

También podemos conectarnos a MySQL utilizando cualquier software gestor de bases de datos, configurando la conexión con los siguientes parámetros:
* Host: localhost
* Port: 3306
* User: user / root
* Password: test / root