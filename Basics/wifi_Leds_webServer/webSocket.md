# ✨ Web Socket  ✨

## Acerca del proyecto

El presente proyecto es un pequeño ejemplo de como controlar remotamente diferente hardware mediante el ESP32, en específico mediante el wifi incluido dentro del mismo SOC 
(System On a Chip). Para ello los principales recursos a necesitar son los siguientes:

## 🚀 Hardware

- Contar con una ESP32 , en este caso la devkit (Incluye wifi y bluetooth) 
- Contar con jumpers o cable para protoboard
- Una protoboard para cablear los respectivos elementos
- Resistencias para los leds (en este caso de 330 ohms)
- Dos leds 

## 🚀 Software

En el caso particular de estre proyecto se empleó el IDE de arduino, sin embargo, esto es a gusto personal.

- Para la conexión del micro con la computadora maestra se empleó la biblioteca "**wifi.h**"
- Para el desarrollo web se empleo HTML5 y algo de CSS básico para hacer un diseño rápido.

## 🚀 Descripción del código

Para una saber más acerca del código y de cómo poder programar en el ESP32, comparto una liga en Youtube, donde se muestra todos estos aspectos y a su vez un ejemplo:
[]()

## Mejoras y consideraciones**

Realmente el hacer que el micro se encargue de desplegar el sitio web, me parece un poco forzado además de muy mal optimizado, esto debido principalmente a 2 factores:
1) Es mandar información redundante además de innecesaria mediante el wifi, realmente lo óptimo sería sólo mandar los estados del led 

2) El front-end debería estar en la computadora maestra y no en la esclava (micro), la esclava solamente debería encargarse de dar los datos.

## Referencias 🤔 

A continuación las ligas usadas para referencia:

1) [https://randomnerdtutorials.com/esp32-web-server-arduino-ide/](https://randomnerdtutorials.com/esp32-web-server-arduino-ide/)
