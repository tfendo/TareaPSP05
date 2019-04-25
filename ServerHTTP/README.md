#TAREA PARA PSP05

##Ejercicio 1

Para realizar este ejercicio tomé como ejemplo el método que devuelve una fecha con el formato adecuado que aparece en la presentación del punto 5.1 y creé el siguiente método:

```
private static String getFecha(){
      DateFormat fecha = new SimpleDateFormat("EEEE, d MMMM yyyy HH:mm:ss z", Locale.ENGLISH);
      fecha.setTimeZone(TimeZone.getTimeZone("GMT+2"));
      return fecha.format(new Date());
  }
```
  
Lo modifiqué para que aparezca el nombre completo del día de la semana y del mes, pero no he conseguido dar con la configuración correcta de localización para que represente bien las tildes en la fecha devuelta, asi que la dejé ajustada al idioma inglés, tal y como aparece en el ejemplo.

Por último añadí la instrucción necesaria para que imprima la cabecera **Date** en cada una de las tres opciones posibles. A continuación presento las capturas correspondientes a cada una de las tres páginas:

![Captura Lenguajes](/Users/HugoGuillin/Desktop/TareaPSP01/Actividad_2/Capturas/Captura4.png) 

![Captura Lenguajes](/Users/HugoGuillin/Desktop/TareaPSP01/Actividad_2/Capturas/Captura4.png) 

![Captura Lenguajes](/Users/HugoGuillin/Desktop/TareaPSP01/Actividad_2/Capturas/Captura4.png) 



##Ejercicio 2
En esta segunda parte me dí cuenta de que había varias instrucciones que no se estaban interpretando correctamente y algunos navegadores no mostraban el contenido, a pesar de que el servidor indicaba que sí lo había servido. He tenido que modificar las instrucciones que fijan el tamaño de la cabezera **Content-Lenght**, poniendo dentro de paréntesis toda la instrucción `html.lenght()+1`, pues sino el uno final lo tomaba como un **String** y lo añadía al final de la frase como un carácter más, en lugar de sumarlo al valor de la longitud de la variable **html**.

En la siguiente captura se puede apreciar como se ejecutan dos consultas en dos navegadores distintos de forma simultánea:

![Captura Lenguajes](/Users/HugoGuillin/Desktop/TareaPSP01/Actividad_2/Capturas/Captura4.png) 