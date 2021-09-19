


# Asus ROG STRIX B460-F Gaming Hackintosh EFI

Este repositorio contiene la carpeta de arranque EFI para la placa madre Asus ROG STRIX B460-F Gaming. El proyecto fue compilado a través de OpenCore para Intel Comet Lake.

Funcionalidades:

- [x] USB 2.0
- [x] USB 3.0
- [x] iServices (iMessage, FaceTime, etc.)
- [x] Wifi
- [x] Bluethoot
- [ ] Airport (Al usar la tarjeta TP-Link TX50E no es posible usar la funcionalidad de Airdrop).

El mapa de puertos USBs está configurado para esta placa teniendo 3 USBs 3.0 (XHC) en la parte trasera de la placa + 1 puerto USB-C (gestionado por un controlador PSXS). En la parte delantera de la placa hay un USB 3.0 (XHC) + 2 puertos USB 2.0 (en HUB, por lo que en la placa cuenta como un solo puerto el cual incluye el puerto Wifi configurado como tipo 255, para uso interno de la placa)

Si vas a copiar y usar en tu máquina Hackintosh toda la carpeta de arranque EFI es necesario que generes una genbios adaptada a ti, de lo contrario la carpeta será inutil. En mi PC estoy usando la SMBIOS iMac20,1 ya que uso un i5-10600K. Para procesadores mayores es necesario usar la GENBIOS iMac20,2. Puedes consultar tus especificaciones en la fantástica guía de [Dortania](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#platforminfo).
