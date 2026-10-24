# Laboratorio 04: Permisos de Linux

## Objetivo

Comprender cómo funcionan los permisos de lectura, escritura y ejecución
en Linux y aplicar el principio de mínimo privilegio.

## Entorno

- Sistema operativo: Ubuntu
- Usuario: cayetano

## Práctica

1. Se creó el archivo `informe.txt` con `touch`.
2. Los permisos iniciales fueron `664` (`rw-rw-r--`).
3. Se ejecutó `chmod 600 informe.txt`.
4. Se verificaron los permisos con `ls -l` y `stat`.
5. Se planteó el permiso `640` como ejercicio.

## Resultados

- `664`: propietario y grupo pueden leer y escribir; otros pueden leer.
- `600`: solo el propietario puede leer y escribir.
- `640`: propietario puede leer y escribir; grupo solo puede leer; otros no tienen permisos.

## Conceptos aprendidos

- `r` = lectura (4).
- `w` = escritura (2).
- `x` = ejecución en archivos y acceso en directorios (1).
- `chmod` modifica permisos.
- `stat` permite verificar permisos.
- El mínimo privilegio reduce accesos innecesarios.

## Limitaciones

Los permisos tradicionales no cifran el contenido y no sustituyen
otras medidas de seguridad.
