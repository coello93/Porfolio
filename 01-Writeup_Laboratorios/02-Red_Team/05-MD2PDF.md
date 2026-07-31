**Completa, Dificultad: Easy** <br> 

Lo que tenemos que hacer en esta maquina es analizar una aplicación web que convierte archivos Markdown (MD) en PDF.<br> 
Nuestro primer paso consiste en entrar en el navegador, y escribir la IP, y se nos muestra el programa.<br> 
<br><img width="1006" height="537" alt="image" src="https://github.com/user-attachments/assets/00061229-7268-4f05-8b0a-376f22777c2e" /><br> 
Si vamos a una terminal, con la herramienta Nmap podemos ver los puertos que están abiertos por si nos da alguna pista.<br>
<br><img width="810" height="330" alt="image" src="https://github.com/user-attachments/assets/996cab6b-14d2-40eb-8ae3-13b779e061bd" /><br>
Podemos observar que están el puerto 22, 80, 5000. <br>
Con la Herramienta de gobuster, vamos  a intenatr enumerar los directorios.<br>
<br><img width="819" height="524" alt="image" src="https://github.com/user-attachments/assets/9f45920c-c350-4f19-ac0e-c7f24d79e9ed" /><br>
vale pone que tiene un directorio admin. Vamos a probar con el, en el navegador<br>
<br><img width="612" height="295" alt="image" src="https://github.com/user-attachments/assets/ee98f8f6-0ba0-438d-ab6a-a45f74132b25" /><br>
Si observamos la imagen nos indica que tenemso que utilizar el puerto 5000. Pero si ponemos la http://IP:5000 Muestra lo mismo<br>
Vamos a escribir esta dirección en el lector de pdf<br>
<br><img width="540" height="186" alt="image" src="https://github.com/user-attachments/assets/36fabdb2-dbfb-4c5d-9779-071a194ca1b1" /><br>
No, parece que no funciona, pero no vamos desencaminados. <br>
<br><img width="808" height="157" alt="image" src="https://github.com/user-attachments/assets/10f09aa8-0ca6-4cf0-803c-e012bc9c2597" />
Vamos a agregar alguna etiqueta de HTML<br>
La etiqueta <iframe> (siglas de Inline Frame o marco flotante) sirve para incrustar un documento HTML completo dentro de otra página web. Probaremos con esto.<br>
<br><img width="644" height="267" alt="image" src="https://github.com/user-attachments/assets/2bfb235c-9e16-408e-81a1-0d8215bf4e2d" /><br>
Pulsamos él botón de convertir a PDF.<br>
<br>Spiler<br>
<br><br>
Conseguimos la Flag, y con esto tenesmo la maquina resuelta.<br> 
<br><img width="596" height="292" alt="image" src="https://github.com/user-attachments/assets/ccc503ae-4540-4d60-9c65-d401431c4181" />


