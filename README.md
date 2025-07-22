# SOCIAL OPLESK
### 
<br/>

# Guía Rápida de Comandos Básicos de Linux

Esta guía proporciona pasos simples y ejemplos concretos sobre los comandos esenciales para quienes comienzan a usar Linux. Incluye explicaciones y el significado de los principales directorios del sistema.

## 1. Listar Directorios y Archivos

- Listar archivos y carpetas en el directorio actual:

```
ls
```

- Listar todo, incluidos archivos ocultos:

```
ls -a
```

- Listar solo directorios:

```
ls -d */
```

o

```
ls -l | grep ^d
```

- Listar con detalles (permisos, fecha, tamaño):

```
ls -l
```


## 2. Buscar Texto con `grep`

- Buscar una palabra en un archivo:

```
grep palabra archivo.txt
```

- Ignorar mayúsculas/minúsculas:

```
grep -i palabra archivo.txt
```

- Buscar recursivamente en carpetas:

```
grep -r palabra .
```

- Mostrar solo las líneas que NO contengan el patrón:

```
grep -v palabra archivo.txt
```


## 3. Moverse Entre Directorios

- Cambiar al directorio `Documentos`:

```
cd Documentos
```

- Ir al directorio principal del usuario:

```
cd ~
```

- Regresar al directorio anterior:

```
cd -
```

- Subir un nivel:

```
cd ..
```


## 4. Crear un Archivo

- Archivo vacío:

```
touch nuevoarchivo.txt
```

- Archivo con contenido:

```
echo "Hola mundo" > texto.txt
```

- Usando un editor como nano o vi:

```
nano archivo.txt
```

o

```
vi archivo.txt
```


## 5. Eliminar un Archivo

- Borrar un archivo:

```
rm archivo.txt
```

- Borrar varios archivos:

```
rm archivo1.txt archivo2.txt
```


## 6. Cambiar el Nombre de un Archivo

- Renombrar (o mover) un archivo:

```
mv viejo.txt nuevo.txt
```


## 7. Crear un Directorio

- Crear el directorio `MisImagenes`:

```
mkdir MisImagenes
```


## 8. Eliminar un Directorio

- Borrar un directorio vacío:

```
rmdir CarpetaVacia
```

- Borrar un directorio y todo su contenido:

```
rm -r CarpetaCompleta
```


## 9. Cambiar el Nombre de un Directorio

- Ejemplo:

```
mv directorio_viejo directorio_nuevo
```


## 10. Instalar un Programa Sencillo (Ubuntu/Debian)

- Actualizar el índice de paquetes:

```
sudo apt update
```

- Instalar un programa (ejemplo: `curl`):

```
sudo apt install curl
```


## 11. Actualizar Sistema de Paquetes

- Para Ubuntu y Debian:

```
sudo apt update
sudo apt upgrade
```


## 12. Crear un Usuario

- Crear usuario nuevo:

```
sudo adduser nombreusuario
```


## 13. Crear un Grupo de Usuarios

- Crear grupo nuevo:

```
sudo addgroup nombregrupo
```


## 14. Significado de los Directorios Básicos en Linux

| Directorio | Significado |
| :-- | :-- |
| / | Raíz, el inicio de toda la estructura |
| /bin | Programas esenciales del sistema |
| /boot | Archivos para el arranque del sistema |
| /dev | Dispositivos del sistema |
| /etc | Archivos de configuración |
| /home | Carpetas de los usuarios |
| /lib | Bibliotecas esenciales |
| /media | Montaje de medios externos (USB, CD, etc.) |
| /mnt | Punto de montaje temporal |
| /opt | Software adicional de terceros |
| /root | Carpeta del usuario root (administrador) |
| /sbin | Programas de administración del sistema |
| /srv | Datos de servicios del sistema (servidores) |
| /tmp | Archivos temporales |
| /usr | Programas y datos de uso general |
| /var | Archivos variables (logs, mail, spool, etc.) |
