# Proyecto Intermodular de VPN

## Descripción
Este proyecto es un trabajo de investigación sobre las Redes Privadas Virtuales (VPN),
su funcionamiento, ventajas, riesgos y casos de uso.
El objetivo es comprender cómo protegen la privacidad y la seguridad en redes públicas.

## Objetivos
- Explicar qué es una VPN y para qué se utiliza
- Analizar cómo funciona el cifrado del tráfico
- Estudiar ventajas y desventajas de usar una VPN
- Comprender los riesgos de privacidad y seguridad

## ¿Qué es una VPN?
Una VPN (Virtual Private Network) crea un túnel cifrado entre el dispositivo del usuario
y un servidor remoto, ocultando la dirección IP real y protegiendo los datos frente a
interceptaciones, especialmente en redes públicas.

## Tecnologías utilizadas
- Tailscale (VPN de malla basada en WireGuard)
- Protocolo VPN: WireGuard
- Cifrado: ChaCha20-Poly1305
- Autenticación: OAuth (Google / GitHub)
- Sistemas operativos: Windows, Linux
- Control de versiones: Git y GitHub

## Headscale
Headscale es un servidor de coordinación open-source compatible con Tailscale
que permite la autogestión de una red VPN de malla basada en WireGuard.

Su función principal es gestionar la autenticación, autorización y coordinación
de los nodos de la red. 

El tráfico de red no pasa por Headscale, sino que se establece directamente entre los dispositivos mediante túneles cifrados
WireGuard, garantizando cifrado de extremo a extremo y baja latencia.

## Funcionamiento
1. El usuario se conecta al servidor VPN
2. Se establece un túnel cifrado
3. El tráfico de red pasa por el servidor VPN
4. La IP real queda oculta y los datos viajan cifrados
5. Los usuarios pueden enviar archivos unos a otros usando tailscale


## Seguridad y limitaciones
- Una VPN no garantiza anonimato total
- El proveedor de VPN puede ver el tráfico
- No protege frente a malware o phishing
