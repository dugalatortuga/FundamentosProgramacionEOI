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

        git commit -am "nombre de la actualizacion"

 



---
---
**_En git tenemos 3 estados:_**
1. _Working directory._ Aquí es donde trabajamos constantemente pero en una etapa aún sin guardar.

2. _Staging area (stage)._ Es una etapa intermedia entre la escritura y la publicación. Podemos enviar nuestro contenido al stage memdiante:
        
         git add .

3. _Repositorio remoto (GitHub)._ Es la etapa final de la información. Con esto ya quedaría publicado. Podemos afianzar el cambio y ponerle nombre mediante:

        git commit -m "nombre de la actualización"
            [master 81f3abd] actualizando
            1 file changed, 92 insertions(+), 6 deletions(-)

* Podemos enviar nuestro contenido del stage al repositorio mediante:
    
        git push main
            Enumerating objects: 5, done.
            Counting objects: 100% (5/5), done.
            Delta compression using up to 4 threads
            Compressing objects: 100% (3/3), done.
            Writing objects: 100% (3/3), 1.28 KiB | 437.00 KiB/s, done.
            Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
            To https://github.com/dugalatortuga/FundamentosProgramacionEOI.git
            42c5d6f..81f3abd  master -> master


Por lo tanto, generaremos el __bucle__ siempre que queramos subir la información trabajada de la siguiente manera:

    - git add .
    - git commit -m "nombre de la actualización"
    (podemos sustituir los dos primeros por git commit -am)
    - git push main


__PARA CONECTAR EL REPOSITORIO LOCAL CON LA NUBE__

git remote add main (y el link del repositorio)

git remote -v para comprobar que la conexión es buena

git push main para conectar
