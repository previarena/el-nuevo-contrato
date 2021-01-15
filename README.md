## Temática: El nuevo contrato

Previred es contactado por el banco internacional Kyrios, debido al gran desempeño que ha tenido en el desarrollo de nuevos productos. Además,
han contactado a tu equipo para poder desarrollar sus proyectos. El banco en cuestión, necesita un proyecto que se entregue con celeridad, ya 
que están teniéndo problemas con el sistema que ya tienen.

El proyecto, consiste en un algoritmo para generar nuevos números de tarjetas de créditos de forma expedita, y han convenido hacerlo en Lisp. El banco te
ha entregado todos los requerimientos y debes comenzar a diseñar y desarrollar.

### Desafío:

Se debe generar un algoritmo para generar 5 nuevos números de tarjetas de crédito para el banco, que cumplan con las siguientes restricciones:

1- Puede contener dígitos de 0 a 9

2- Debe ser de largo 16

3- No deben repetirse las tarjetas de crédito.

4- Deben ser válidos según el algoritmo de Luhn, el cuál se explica a continuación: 

Para validar un número de tarjeta utilizando el algoritmo de Luhn se deben seguir estos pasos:

1-Se multiplica cada dígito de posición par (contando desde la derecha) por dos. Si el resultado es un número de dos dígitos, entonces se suman estos dos valores

2-Posteriormente, se suman todos los dígitos obtenidos

3-Luego esa suma se divide entre 10, y si el resto de la división es 0 entonces es un número válido.

![alt text](https://raw.githubusercontent.com/previarena/el-nuevo-contrato/main/luhn.PNG)

[Si no puede visualizar la imágen, puede verla haciendo click en luhn.PNG dentro del mismo proyecto]

Las tarjeta además se componen de una estructura, del siguiente tipo:

![alt text](https://www.mobilefish.com/images/services/bank_identification_number_creditcard.png)

[Si no puede visualizar la imágen, puede verla haciendo click en formatoTarjeta.png dentro del mismo proyecto]

donde primero se encuentra la id del banco, que en el caso del banco Kyrios es: 579826, luego se encuentra el número de cuenta que tenemos que generar
y el dígito 16 es el dígito verificador, que se ocupa para validar que los demás números sean correctos.

Esta vez no tenemos entrada de datos, sin embargo, la salida deben ser los 5 números válidos de las tarjetas de crédito del banco Kyrios del siguiente modo:

| Ejemplo de salida              |                
|--------------------------------|
|  5798 26XX XXXX XXXY           |
|  5798 26XX XXXX XXXY           |
|  5798 26XX XXXX XXXY           |
|  5798 26XX XXXX XXXY           |
|  5798 26XX XXXX XXXY           |


Motivación: El algoritmo de Luhn es utilizado para validar los números de las tarjetas de créditos hasta el día de hoy.

Ánimo Previdiano, ya termina la semana, 
aprovecha de hacer amigos y aprender en el proceso!.
