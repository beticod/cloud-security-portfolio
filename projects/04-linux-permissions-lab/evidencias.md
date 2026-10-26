# Evidencias — Linux File Permissions Lab

## Entorno
- Sistema operativo: Ubuntu Linux
- Herramientas: chmod, ls, stat
- Objetivo: comprender los permisos tradicionales de Linux.

## Prueba 1: permisos iniciales

Comando ejecutado:
`touch informe.txt`

Resultado observado:
- Permisos: 664 (`rw-rw-r--`)
- Propietario: cayetano
- Grupo: cayetano

Interpretación:
El propietario y el grupo tienen lectura y escritura.
Otros usuarios tienen permiso de lectura.

## Prueba 2: restricción de acceso

Comando ejecutado:
`chmod 600 informe.txt`

Resultado observado:
- Permisos: 600 (`rw-------`)

Interpretación:
Solo el propietario tiene permisos de lectura y escritura.

## Prueba 3: análisis de permisos 640

- Propietario: lectura y escritura.
- Grupo: solo lectura.
- Otros: sin permisos.

Este permiso se analizó como ejercicio teórico.

## Conclusión

La práctica demuestra cómo reducir los permisos de un archivo
y aplicar el principio de mínimo privilegio.

## Limitaciones

Los permisos tradicionales no cifran el contenido y no sustituyen
otras medidas de seguridad.
