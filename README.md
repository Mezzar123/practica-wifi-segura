# practica-wifi-segura
# Pre entregable 6 — Informe de auditoría de red Wi-Fi insegura

## Introducción

En esta ocasión vamos a realizar un trabajo de "Informe de auditoría de red Wi-Fi insegura", donde vamos a aplicar nuestros conocimientos y habilidades de análisis de tráfico para documentar riesgos reales de una red Wi-Fi pública.

La idea es simular el trabajo de un auditor de seguridad junior, identificando una vulnerabilidad y proponiendo una posible solución.

## Sitio analizado

El sitio utilizado para realizar el análisis fue:

**http://neverssl.com**

### Datos de la solicitud

- **URL solicitada:** `http://splendidsublimesilverspell.neverssl.com/online/`
- **Método HTTP:** `GET`
- **Host:** `splendidsublimesilverspell.neverssl.com`
- **Protocolo utilizado:** `HTTP/1.1`
- **Headers enviados:** `text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7`

## Evidencia observada

Durante la solicitud pude observar diferentes datos de la comunicación. Me voy a centrar principalmente en tres elementos: **URL, Host y User-Agent**.

### URL

Indica la dirección exacta a la que se está realizando la solicitud. En este caso:

`http://neverssl.com/`

### Host

Indica el servidor o sitio al que se está conectando el navegador. En este caso:

`splendidsublimesilverspell.neverssl.com`

### User-Agent

Muestra información sobre el navegador y el sistema operativo que estoy utilizando para realizar la solicitud. En este caso, el navegador utilizado es **Chrome** y el sistema operativo es **Windows 11**.

## Riesgos encontrados

El sitio utiliza **HTTP y no HTTPS**. Esto significa que la comunicación entre el navegador y el servidor no está cifrada.

Navegar mediante HTTP en una red Wi-Fi pública puede ser riesgoso porque la información que se transmite no está cifrada. Un atacante que esté en la misma red podría llegar a interceptar datos como las páginas que visito, las solicitudes que realizo y otra información que se esté enviando.

Por eso es más seguro utilizar sitios que tengan **HTTPS**, especialmente cuando se manejan datos personales o información sensible.

## Cómo ayuda una VPN

Una VPN puede ayudar a proteger la conexión mediante diferentes mecanismos:

### Cifrado

Protege la información transformándola para que no pueda ser leída fácilmente por terceros durante la comunicación.

### Túnel seguro

Es una conexión protegida que se crea entre mi dispositivo y el servidor de la VPN. Por este túnel viajan mis datos de forma cifrada, evitando que otras personas en la misma red puedan acceder fácilmente a ellos.

### Protección del tráfico

Significa que la VPN protege los datos que envío y recibo mientras navego, evitando que puedan ser vistos o interceptados fácilmente por otras personas que estén en la misma red.

### Privacidad

La VPN ayuda a proteger mi privacidad al ocultar mi dirección IP real y dificultar que terceros puedan saber directamente desde dónde me estoy conectando o seguir mi tráfico en la red.

## 3 Reglas de Oro

Mis 3 reglas de oro para navegar por Internet mediante una Wi-Fi pública son:

1. **Evitar ingresar datos sensibles**, como contraseñas o información bancaria, cuando estoy conectado a una Wi-Fi pública.

2. **Usar HTTPS o una VPN** para proteger la información que envío y recibo mientras navego.

3. **Desactivar la conexión automática a redes Wi-Fi**, para evitar conectarme sin darme cuenta a redes desconocidas.
