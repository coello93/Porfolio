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
<br>
