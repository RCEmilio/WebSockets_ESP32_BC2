# Cuestionario de Evaluación: Comunicación por Sockets 📝

**Nombre del Estudiante:** Emilio Ruiz
**Fecha:** 25-03-26

*Instrucciones: Responde a las siguientes preguntas basándote en la teoría de redes y en el análisis del código de nuestro proyecto. Sube este archivo con tus respuestas a tu repositorio como evidencia de trabajo.*

1. **¿Qué es una Dirección IP y para qué sirve en nuestro proyecto?**
   > *Tu respuesta aquí*
Es aquel identificador que tiene única y exclusivamenre cada dispositivo que nos ayudará y permitirá conectar el dispositivo ESP32
2. **¿Qué es un Puerto de red? (Menciona qué puerto estamos usando en el código de la ESP32).**
   > *Tu respuesta aquí*
Nosotros usamos el puerto 80 y es el numero que identifica el servicio 
3. **Define con tus propias palabras qué es un Servidor en informática.**
   > *Tu respuesta aquí*
Programa que envia datos a diversos equipos y que esta a la espera de señales 
4. **¿Cuál es la diferencia entre un "Servidor" (Hardware/Software) y un "Servicio" (Service)?**
   > *Tu respuesta aquí*
Un servidor es quien ejecuta el sistema y el servicio es en cambio la función que realiza 
5. **Investigación: ¿Cuál es la diferencia técnica entre un "Socket TCP" normal y un "WebSocket"?**
   > *Tu respuesta aquí*
Webosocket ayuda ala comunicación en tiempo real sobre la web y TCPes una conexión directa a los datos
6. **Analizando nuestro código: ¿Quién actúa como Servidor y quién actúa como Cliente? (Justifica tu respuesta mencionando qué funciones del código lo demuestran, ej. `bind()`, `connect()`).**
   > *Tu respuesta aquí*
ESP32 es el servidor y el cliente el dispositivo porque utilizamos connect() para realizr la conexión
7. **En el código de la computadora (Python), importamos la librería `threading` (Hilos). ¿Qué pasaría con la ventana de Tkinter si no usáramos hilos para recibir los datos de la red?**
   > *Tu respuesta aquí*
Probablemente se quedaría estático ya que no posee los datos de la red y se encuentra en espera de los mismos
8. **¿Por qué es necesario usar bloques `try...except` cuando trabajamos con conexiones de red e Internet?**
   > *Tu respuesta aquí*
Para ver los posibles errores en nuestra conexión y que asi el programa no se cierre 
9. **En la función de encender el LED en Python, enviamos el comando así: `sock.send(b'ON')`. ¿Qué significa esa letra `b` antes de las comillas y por qué no enviamos un texto normal?**
   > *Tu respuesta aquí*
Que se envian los bytes ya que los sockets utilizan datos binarios 
10. **Describa brevemente el flujo de datos: ¿Que camino recorrre la informacion desde que gira el potencionmeto basicamente hasta que la barra se mueve en la pantalla de la computadora?**
   > *Tu respuesta aquí*
El potenciometro envia un valor al ESP32, mandandolo via red mediante sockets, para luego que los reciba la computadora y actualiza la barra en Tkinter


10. **Describe brevemente el flujo de datos: ¿Qué camino recorre la información desde que giras el potenciómetro físicamente hasta que la barra se mueve en la pantalla de la computadora?**
    > *Tu respuesta aquí*
