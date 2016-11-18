# Introducción

Kinton es una herramienta diseñada para simplificar la comunicación entre dispositivos en el Internet de las Cosas. 

Si buscamos soluciones ya desarrolladas se pueden encontrar varias alternativas, muchas de ellas realizadas por empresas de la talla de IBM o AT&T que son maduras y ofrecen todo lo necesario. Sin embargo, todas ellas atan al usuario a usar su infraestructura y depender de ella, si el usuario decide que ya no le conviene seguir usando el servicio puede ser un problema migrar a otro.

# Introducción

Usuario
Se llamará usuario a la persona, personas u organización que utiliza la plataforma que vamos a diseñar para

su beneficio. Se pretende cubrir una necesidad, que en este caso es comunicar dos elementos: los dispositivos

integrados del usuario y la lógica de negocio del usuario.

El usuario no tiene por qué saber cómo funciona el sistema de forma interna, sólamente deberá saber cómo

interactuar con él.

Dispositivos integrados

En primer lugar se encuentran los dispositivos del usuario, que son los elementos que se pretenden dotar de

conectividad para que puedan comunicarse de forma eficiente y robusta. Se debe tener en cuenta que cuando

se habla de sistemas integrados no se puede suponer que se cuenta con los mismo recursos que en un equipo

estándar. La cantidad de memoria, de almacenamiento, de ancho de banda o incluso de energía pueden ser

muy limitadas, por lo que no se pueden aplicar las mismas soluciones que se aplicarían en un entorno donde

sobran dichos recursos.

Con esto se quiere decir que protocolos como ❍❚❚P que funcionan de forma correcta en un equipo actual

no tienen por qué funcionar igual de bien en un dispositivo que cuenta con poca memoria. Si en lugar de

WiFi se usa un protocolo más simple orientado a eficiencia energética, ❍❚❚P puede ser muy pesado y su

implementación puede consumir mucha memoria, energía o ancho de banda.

Habrá que buscar soluciones acordes a esta tecnología.

Lógica de negocio

Es el conjunto de software que desea comunicarse con los dispositivos, ya sea para recolectar los datos que

unos sensores captan o para accionar unos actuadores. Toda esta lógica pertenece al usuario y puede ser

desde un pequeño script en Python hasta una compleja infraestructura desplegada en Amazon. Puesto que

tiene otras características diferentes a los dispositivos tendrán otros requisitos diferentes, por lo que la forma

en la que interaccionarán con la plataforma no tiene por qué ser la misma que los dispositivos.

Uno de los requisitos para la lógica de negocio es que debe poder funcionar en un navegador web, de forma

que se podría crear una aplicación web que se comunique directamente con la plataforma.
