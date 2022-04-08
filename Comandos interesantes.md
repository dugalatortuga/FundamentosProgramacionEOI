# COMANDOS INTERESANTES PARA LA CONSOLA
---
__NAVEGACIÓN ENTRE DIRECTORIOS__

- Mostrar el contenido de la carpeta, tanto visible como oculto en el explorador de Windows:

        dir

- Acceder a una carpeta (change directory)

        cd + nombre de la carpeta


- Volver a la carpeta anterior (volvemos carpeta a carpeta)

        cd ../

- Ir a la carpeta raiz (normalmente C:)

        cd /

- Limpiar pantalla, pero sin perder los comandos realizados (clear screen):

        cls

- Borrar archivo

        del + nombre del archivo.extensión (todo sin paréntesis)

- Crear nueva carpeta

        mkdir + nombredelacarpeta (sin espacios en el nombre)


        
---


__COMANDOS PARA GIT__


![COMANDOSBASICOS](img/04.jpg)


- Comprobar que tenemos instalado git:

        git

- Iniciar repositorio:

        git init

- Añadir todos los archivos desde el último commit:

        git add .

- Revertir git add .

        git reset .

- Visualizar los cambios hechos y enviados a commit:

        git log

- Crear una nueva rama en el árbol

        git checkout -b +NombreDeLaRama


- Combinación de _git add. + git commit -m_

        git comit -am

 



---
---
**_En git tenemos 3 estados:_**
1. _Working directory._ Aquí es donde trabajamos constantemente pero en una etapa aún sin guardar.

2. _Staging area (stage)._ Es una etapa intermedia entre la escritura y la publicación. Podemos enviar nuestro contenido al stage memdiante:
        
         git add .

3. _Repositorio remoto (GitHub)._ Es la etapa final de la información. Con esto ya quedaría publicado. Podemos afianzar el cambio y ponerle nombre mediante:

        git commit -m

* Podemos enviar nuestro contenido del stage al repositorio mediante:
    
        git push main


Por lo tanto, generaremos el __bucle__ siempre que queramos subir la información trabajada de la siguiente manera:

    - git add .
    - git commit -m
    (podemos sustituir los dos primeros por git commit -am)
    - git push main








