# Actividad: Trabajando con Permisos en Linux

## Objetivo

Esta actividad tiene como objetivo que los estudiantes comprendan y practiquen la gestión de permisos en Linux, utilizando los comandos `chmod`, `chown` y `ls`.

## Instrucciones

### 1. Preparación

1. Abrí una terminal en tu distribución de Linux.
2. Crea un directorio llamado `actividad_permisos` y accede a él.

```sh
mkdir actividad_permisos
cd actividad_permisos
```
### 2. Creación de Archivos y Directorios
Dentro del directorio actividad_permisos, crea los siguientes archivos y un subdirectorio:
```sh
touch archivoA.txt archivoB.txt archivoC.txt
mkdir subdirectorio
```
### 3. Exploración de Permisos
Usa el comando ls -l para ver los permisos actuales de los archivos y directorios creados.
```sh
ls -l
```
2. Anota los permisos actuales de cada archivo y directorio en la siguiente tabla:

| **Nombre**      | **Permisos Actuales** |
|-----------------|-----------------|
| archivoA.txt	  |   -rw- rw- r--  |
| archivoB.txt    |   -rw- rw- r--  |
| archivoC.txt    |   -rw- rw- r--  |
| subdirectorio   |   drwx rwx r-x  |

### 4. Modificación de Permisos
Cambia los permisos de archivoA.txt para que el usuario tenga permisos de lectura y escritura, el grupo solo lectura y otros no tengan permisos.

```sh
chmod 640 archivoA.txt
```


Cambia los permisos de archivoC.txt para que el usuario tenga todos los permisos, el grupo solo lectura y otros solo ejecución.

```sh
chmod 741 archivoC.txt
```

Cambia los permisos del subdirectorio para que el usuario tenga todos los permisos, el grupo y otros solo tengan permisos de lectura y ejecución.
```sh
chmod 755 subdirectorio/
```
### 5. Verificación de Cambios
```sh
ls -l
```
Anota los nuevos permisos de cada archivo y directorio en la siguiente tabla:

| **Nombre**      | **Permisos Actuales** |
|-----------------|-----------------|
| archivoA.txt	  |   -rw- r-- ---  |
| archivoB.txt    |   -rw- rw- r--  |
| archivoC.txt    |   -rwx r-- --x  |
| subdirectorio   |   drwx r-x r-x  |

### 6. Cambio de Propietarios
1. Cambia el propietario de archivoA.txt a otro usuario (reemplaza otro_usuario con el nombre de un usuario existente en el sistema o crealo).
```sh
chown pepito archivoA.txt
```
3. Cambia el grupo de archivoB.txt a otro grupo (reemplaza otro_grupo con el nombre de un grupo existente en el sistema o crealo).
```sh
chown :tennis arhivoB.txt
```
5. Cambia el propietario y grupo de archivoC.txt a otro_usuario y otro_grupo.
```sh
chown pepito:tennis archivoC.txt
```
### 7. Verificación de Cambios de Propietarios
1. Usa el comando ls -l para verificar los cambios en los propietarios y grupos.
2. Anota los nuevos propietarios y grupos de cada archivo en la siguiente tabla:

| **Nombre**      | **Nuevo propietario** | **Nuevo grupo**|
|-----------------|-----------------------|----------------|
| archivoA.txt	  |        pepito         |   ubuntu-mate  |
| archivoB.txt    |      ubuntu-mate      |     tennis     |
| archivoC.txt    |        pepito         |     tennis     |
| subdirectorio   |      ubuntu-mate      |   ubuntu-mate  |

### 8. Reflexión
¿Qué diferencias observaste en el comportamiento de los archivos y directorios al cambiar sus permisos y propietarios?
Al cambiar los permisos y propietarios observer que en algunos casos no podia acceder y/o escribir en ellos y en otros casos que quise modificar sus permisos no me dejaba ya que no era el propietario de los archivos

¿Por qué es importante gestionar correctamente los permisos en un sistema Linux?
Es importante gestionar correctamente los permisos en Linux ya que podrias tener un problema con algunos archivos del sistema en el que no te deje acceder al mismo, teniendo que reinstalar nuevamente el Sistema Operativo
