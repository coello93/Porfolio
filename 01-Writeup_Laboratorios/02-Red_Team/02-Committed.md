**Completada, Dificultad: Easy**<br>

En esta maquina nos indican que alguien ha subido por error al Github un codigo confidencial. Y nosotros tenemos que analizar que ha subido. <br>

Lo que tenemos que hacer es iniciar nuestras maquinas, y descomprimir la carpeta commited. <br>

Vemos solo esto, pero nosotros desde la terminal podemos ver carpetas ocultas. <br> <img width="628" height="236" alt="image" src="https://github.com/user-attachments/assets/0e6b2382-34e7-45a4-b451-028d33423f04" /> <br>

Para ver las carpetas ocultas insertamos el comando ls -la <br>
<img width="511" height="167" alt="image" src="https://github.com/user-attachments/assets/86f8b4e5-dba1-47aa-b85a-649bb149a54c" />
<br>
Depues de entrar dentro de la carpeta oculta, segimos viendo mas archivos y mas directorios. Entramos en la carpeta logs. Observamos que tiene un archivo, vamos abrirlo conel coamdno cat para no modificar su información.<br>
<img width="947" height="513" alt="image" src="https://github.com/user-attachments/assets/3bdd74b9-dc3e-4345-bd26-3bcf17960825" /> <br>
Si observamos hay tenemso un comentario que indica Oops (Parece que alguien se dio cuenta que la lio)<br>
Vamos a copiar ese codigo. c56**********************
<br>
Ahora tenemos que saber algunos comando de git. Si no podemos hacer git -help o git help -a (Para encontrar mas ayuda sobre este comando) 
<br>
**Nota:** Lo importante no es completar maquinas, es comprenderlo y aprender en el proceso, buena suerte.<br>
<br>
**Solucion.** <br>

Si utilizamos el comando git show c56c470a2a9dfb5cfbd54cd614a9fdb1644412b5 podemos observar la flag.<br>
<br>
<img width="943" height="521" alt="image" src="https://github.com/user-attachments/assets/9aa9e598-742c-4803-a18b-95b512fddaab" />
<br>
**Enhorabuena, lo conseguiste.**
