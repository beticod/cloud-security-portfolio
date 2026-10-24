# Fundamentos de Linux y redes

## Entorno
- Sistema operativo: Ubuntu 26.04.1 LTS
- Arquitectura: x86_64
- Usuario: cayetano

## Red
- Interfaz Ethernet: enp5s0
- Dirección IPv4: 192.168.24.75/24
- Puerta de enlace: 192.168.24.4
- Interfaz Wi-Fi: wlp3s0 (inactiva durante la práctica)

## Comandos aprendidos
- pwd: muestra el directorio actual.
- ls -la: muestra archivos y permisos.
- id: muestra usuario, UID y grupos.
- ip -br address: muestra las interfaces y sus direcciones.
- ip route: muestra las rutas de red.
- ping: comprueba la conectividad mediante ICMP.
- getent hosts: permite comprobar la resolución de nombres.
- curl: realiza peticiones a servidores web.

## Prueba de conectividad

- DNS: getent hosts example.com devolvió direcciones IPv6.
- HTTPS: curl -I https://example.com devolvió HTTP/2 200.
- Conclusión: la resolución DNS funcionó y se pudo realizar una petición HTTPS.
- IPv4 e IPv6: son dos formatos de direcciones IP.
