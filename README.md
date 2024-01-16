# TOCACO2
Trabajo sobre documentación de gestión de repositorios o algo así

## Trabajo realizado por Javier Cotillas, Alejandro Costa, Domingo Cabrero y Ángel Toledo

# Parte 1 

### ¿Cómo podemos crear un repositorio remoto?
    
Para llevar nuestro repositorio local a un repositorio remoto, primero tenemos que crear un repositorio en GitHub que para hacerlo debemos ir al DashBoard de nuestro GitHub y en la parte derecha nos saldrá un + que al darle ahi nos llevará a un menú: ![image](https://github.com/SandeyDAM/TOCACO2/assets/149526445/f04967cf-11cd-4963-b614-540eefdf5dc3)

Donde aqui podremos ver: 
- Nombre: Pondremos el nombre del repositorio
- Descripción: Es opcional, podemos describir lo que haremos en nuestro repositorio
- Privacidad del repositorio: Ahí pondremos si queremos que nuestro repositorio sea privado o público.
- Inicializar un ReadME
- Añadir un .gitignore
- Añadir una licencia 

 ***Una vez hecho todos estos pasos lo siguiento es irnos a nuestro terminal;***

 Aqui para comenzar lo que tenemos que hacer es añadir la dirección del repositorio remoto a nuestro repositorio local, para ver nuestra dirección tenemos que irnos al panel principal de nuestro repositorio buscar está opción ![image](https://github.com/SandeyDAM/TOCACO2/assets/149526445/37003cb9-7d3a-4d75-90eb-e946ed853900)
Y ahi encontraremos la dirección.

Una vez encontrada nuestra dirección debemos poner el siguiente comando:
    
    $ git remote add origin <url de nuestro repo>

 
***También podemos crear un repositorio local a partir de uno remoto;***

 Está opción la debemos usar cuando hemos creado el repositorio en GitHub pero todavia no tenemos un repositorio, en este caso debemos usar el comando git clone para clonar todos los datos del GitHub a nuestro repositorio local.

     $ git clone <url de nuestro repo>

Este mediante protocolo HTTP.

    $ git clone <url de nuestro repo>

Este por ssh.

Y estas maneras son las que tenemos para crear un repositorio remoto.

### ¿Qué es el README.md?

Los archivos readme son archivos que contienen información importante sobre el sistema, proyecto o software al que hacen referencia. Debido a su utilidad, se recomienda ubicarlo en el nivel superior del directorio para que sea fácil de encontrar por los usuarios.

### Sobre Markdown

- Markdown es un lenguaje de marcado sencillo que sirve para agregar formato, vínculos e imágenes con facilidad al texto simple

- Nació como una herramienta de conversión de texto plano a HTML. Se distribuye de manera gratuita bajo una **licencia BSD**.

- También se considera un lenguaje que tiene la finalidad de permitir crear contenido de una manera sencilla de escribir, y que en todo momento mantenga un diseño legible, así que para simplificar puedes considerar Markdown como un método de escritura.

- Los comandos de Markdown son admitidos por el editor de tickets de manera automática. Se pueden ingresar comandos de Markdown para formatear el contenido o, si se prefiere, se puede usar la barra de herramientas de formato para agregar contenido enriquecido

- Este tipo de formato siempre será compatible con todas las plataformas que utilices, así que utilizar Markdown es una manera de mantener todo tu contenido siempre accesible desde cualquier dispositivo.

### ¿Qué son y qué utilidad tienen las licencias?
Las licencias son permisos que informan a las demás personas de lo que pueden hacer y lo que no con tú codigo fuente.

Hay distintos tipos de licencias:

- Licencia MIT: Es una licencia de software permisiva, es decir, marca pocas limitaciones en la reutilización de código. Por lo que posee  una compatibilidad de licencia muy buena. También permite reutilizar software dentro del software propietario. Es compatible con licencias copyleft, como la GNU(el software con licencia MIT puede integrarse en software con licencia GPL, pero no viceversa).

- Licencia GNU GPL: Es una licencia de software libre que garantiza a los usuarios finales la libertad de usar, estudiar, compartir y modificar el software. Tiene dos propósitos: declarar que el software cubierto por esta licencia es libre, y protegerlo de intentos de apropiación que restrinjan esas libertades a nuevos usuarios cada vez que la obra es distribuida, modificada o ampliada (mediante una práctica conocida como copyleft) .

- Licencia Apache:  Es una licencia de software libre permisiva, pero no es una licencia copyleft, ya que no requiere la redistribución del código fuente cuando se distribuyen versiones modificadas.
Al igual que las anteriores, otorga al usuario la libertad de usar el software para cualquier propósito, re distribuirlo, modificarlo y distribuir versiones modificadas del software.

- No License: Se produce cuando no ponemos licencia en nuestro pryecto. En este caso se aplican las leyes de derecho de autor predeterminadas, lo que implica que se conservan todos los derechos del código fuente, y nadie puede reproducir, distribuir o crear trabajos a partir de éste. 



  
### ¿Qué es el fichero .gitignore?

Gitignore es una herramienta utilizada en Git para excluir archivos y directorios del control de versiones. Ayuda a los usuarios a mantener sus repositorios limpios y organizados evitando que se rastreen archivos innecesarios.

Consiste en un archivo de configuración que contiene una lista de patrones donde se especifican archivos o directorios que Git debe ignorar.
Sigue una sintaxis en la que los patrones pueden incluir comodines (*), negación (/) y comentarios (#). Dependiendo de su ubicación en el proyecto, los archivos Gitignore pueden ser locales, globales o a nivel de repositorio.

Para crear estos archivos, basta con crear un archivo de texto plano con el nombre .gitignore en el directorio root de tu repositorio Git.

Acto seguido, los usuarios podrán especificar los archivos o directorios que deseen ignorar utilizando patrones Gitignore. Por ejemplo, para ignorar todos los archivos .txt en un directorio llamado price_list, puedes crear un archivo Gitignore con el siguiente contenido:

    *.txt 
    price_list/


### Tres formas de integrar el repositorio remoto en un repositorio local.


La primera forma de integrar un repositorio remoto a un repositorio local es clonando el repositorio remoto. 


    git clone <repo url>

Al ejecutar git clone, tienen lugar las siguientes acciones:

- Se crea una carpeta con el nombre repo
- Esta carpeta se inicializa como un repositorio de Git.
- Se crea un repositorio remoto denominado origin, que apunta a la dirección URL desde la que ha realizado la clonación
- Todos los archivos y confirmaciones del repositorio se descargan aquí.
- La rama predeterminada está desmarcada

La segunda forma es fusionar cambios en tu rama local.

Esta forma consiste en combinar tus cambios locales con los cambios realizados por otros, es decir combina tu repositorio local con el repositorio remoto.

    $ git merge REMOTE-NAME/BRANCH-NAME

La tercera forma consiste en extraer los cambios de un repositorio remoto a un repositorio local.

git pull es un método abreviado útil para completar git fetch y git mergeen el mismo comando:

    $ git pull REMOTE-NAME BRANCH-NAME




### ¿Comó realizar un commit?

Consolidar, confirmar o hacer un commit se refiere a la idea de confirmar un conjunto de cambios provisionales de forma permanente.

Esto se hace a través del comando git commit. El cual captura una instantánea de los cambios preparados en ese momento del proyecto. Las instantáneas confirmadas pueden considerarse como versiones "seguras" de un proyecto: Git no las cambiará nunca a no ser que se lo pidas expresamente. Antes de ejecutar git commit, se utiliza el comando git add para pasar o "preparar" los cambios en el proyecto que se almacenarán en una confirmación. Estos dos comandos, git commit y git add, son dos de los que se utilizan más frecuentemente.

Otras opciones igualmente comunes 

    git commit
    
Confirma la instantánea preparada. El comando abrirá un editor de texto que te pedirá un mensaje para la confirmación. Una vez escrito el mensaje, guarda el archivo y cierra el editor para crear la confirmación.

    git commit -a

Confirma una instantánea de todos los cambios del directorio de trabajo. Esta acción solo incluye las modificaciones a los archivos con seguimiento (los que se han añadido con git add en algún punto de su historial).

    git commit -m "commit message"

Un comando de atajo que crea inmediatamente una confirmación con un mensaje de confirmación usado. De manera predeterminada, git commit abrirá el editor de texto configurado localmente y solicitará que se introduzca un mensaje de confirmación. Si se usa la opción -m, se omitirá la solicitud de editor de texto a favor de un mensaje insertado.

    git commit -am "commit message"
    
Un comando de atajo para usuarios avanzados que combina las opciones -a y -m. Esta combinación crea inmediatamente una confirmación de todos los cambios preparados y aplica un mensaje de confirmación insertado.

    git commit --amend

Esta opción añade otro nivel de funcionalidad al comando confirmado. Al pasar esta opción, se modificará la última confirmación. En vez de crear una nueva confirmación, los cambios preparados se añadirán a la confirmación anterior. Este comando abrirá el editor de texto configurado del sistema y te pedirá que cambies el mensaje de confirmación especificado anteriormente.







### ¿Cada cuanto hay que realizar un commit?
Un commit se debe realizar cada vez que quieras confirmar un cambio en tu proyecto, es decir, ¿Acabas de añadir una nueva funcionalidad a tu programa?, pues en ese momento deberias realizar un commit con todos los cambios añadidos. Debes tener en cuenta que estos siempre se deben hacer una vez este esta nueva funcionalidad totalmente testeada y estes seguro de querer implementarla a tu proyecto.


### ¿Cómo podríamos trabajar varias personas en el mismo proyecto?

Para poder trabajar varias personas en el mismo proyecto de GitHub, lo que debemos hacer es:

En nuestro repositorio nos iremos a la configuración del mismo y allí, nos vamos al apartado llamado *Access*, donde encontraremos la pestaña llamada *Collaborators* donde desde alli podremos añadir a todos los colaboradores que queremos que se añadan a nuestro proyecto.



# Parte 2 

### Creación de ramas.

Para poder crear una rama en git debemos usar el **git branch**:

    git branch <nombre de la rama>

Para cambiar entre ramas:

    git checkout <nombre de la rama>

Para borrar una rama:

    git branch -d <nombre de la rama>

Forzando borrado:

    git branch -D <nombre de la rama>


### Proceso de merge entre ramas.

El proceso de merge consiste en combinar o fusionar ramas con el objetivo de llevar todos los cambios que se han realizado(errores, nuevas funcionalidades...) a la rama principal(main) o a una superior.

Para poder mergear una rama a otra tenemos que usar el comando merge:

    git merge <nombre de la rama>

Con este comando estaremos mergeando la rama que elijamos con la rama superior. En este proceso la rama que hemos elejido se sobreescribe en la rama superior, pero no se elimina.

Si se desea eliminar la rama una vez mergeada nos situamos en otra rama con el comando checkout:

    git checkout <nombre de la otra rama>    
    
y ejecutamos el comando brnach -d para eliminarla:

    git branch -d <nombre de la rama>

### Resolución de conflictos en un merge.

Algunas veces la unión de dos ramas no funciona, sino que ocurre un conflicto. Esto ocurre cuando los commits de la rama a fusionar, y la rama actual, modifican la misma parte en un archivo en particular y git no puede decidir cuál versión elegir. Por lo que te avisa de que tu debes resolverlo. Por ejemplo:
Supongamos que un directorio tenemos un archivo index.html con el siguiente contenido:

    <!DOCTYPE HTML>
    <html>
      <head>
        <title>Titulo</title>
      </head>
      <body>
        <p>Contenido de la web</p>
      </body>
    </html>

Inicializaremos un repositorio haciendo git init y luego haremos nuestro primer commit con: 

    git add index.html 

Y luego:

    git commit -m “commit inicial”

Vamos a crear una nueva rama para añadir algo de contenido:

    git checkout -b contenido

Con ello ya estamos en la nueva rama y ahora vamos a cambiar el título. Guardamos los cambios y hacemos commit en esa rama: 

    git commit -a -m “cambios en el titulo”

Nos movemos de nuevo a la rama master:

    git checkout master

Hacemos otros cambios en el archivo incluyendo el título y luego commit de los cambios:

    git commit -a -m “se añade más contenido”

Ahora intentamos hacer merge con la rama creada anteriormente:

    git merge contenido

En este caso no podrá hacer el merge y nos mostrará que hay un conflicto que no nos permitirá continuar hasta que se resuelva:

Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.

Git no proporciona una ayuda diciéndonos que archivo tiene el conflicto, el cual al abrirlo nos muestra cuáles son los cambios tanto de una rama como de la otra:

![image](https://styde.net/wp-content/uploads/2015/10/conflicto-con-git-merge.png)


donde tenemos que elegir entre lo que está entre <<<<<<< HEAD y ======= que es contenido que tenemos en la rama donde estamos haciendo el merge (master) o entre ======= y >>>>>>> contenido donde están los cambios hechos en la rama que queremos unir (contenido). 

Para ello arreglamos el archivo con los cambios elegidos, guardamos, agregamos y hacemos commit de los cambios:

    git commit -a

y de esta manera lograremos hacer merge con éxito.

Otra manera para resolver conflictos es indicando de antemano a git que estrategia tomar cuando tiene que decidir ante un conflicto. Esto se hace con las opciones ours y theirs, de esta manera:

    git merge -s recursive -X theirs rama-a-fusionar

Esto cuando queremos que git resuelva el conflicto usando los cambios de la rama a fusionar (theirs o suyos) y cuando queremos que tome los cambios de la rama donde se está fusionando (ours o nuestros): 

    git merge -s recursive -X ours rama-a-fusionar



### Diferencias entre un pull y un fetch.

La diferencia esta en que:

Con ***git fetch*** descargaremos el contenido remoto sin modificar el estadod del repo local, que lo diferencia con ***git pull***, que descargará el contenido que está en remoto y tratará inmediatamente de cambiar el estado en el que se encuentra el repositorio local, para asi poder enseñar ese contenido. Y esto podrá, de manera accidental provocar un conflicto dentro del repositorio local.

### ¿Cómo podríamos volver a una versión anterior del proyecto?


Para deshacer y rehacer cambios en Git, existe el comando:

    git reset

Que tiene tres formas de invocación: --hard, --mixed y --soft.

Con la primera forma --hard, lo que hará es retroceder al sistema en su linea de dependencia hasta la version que le diga el programador.

    git reset --hard <version>

Si queremos saber el historial del respositorio y ver que cambios deshizo el comando, deberás poner el comando:

    git log

Otra manera que tenemos para regresar es usando la clave única:

    git reset --hard <version> <clave>

Es importante saber que, git nunca va a eliminar nada y que cada versión tendrá su clave única. Así que, por muchos cambios que deshagas o hagas, siempre habrá un backup.

Para poder recuperar las versiones que deshiciste en un paso anterior, debes utilizar el comando: *git reflog*. 
Al usar este comando de esta manera:

    git reflog

Nos devolvera un listado con todos los movimientos realizados del más moderno al mas antiguo, donde también encontraremos los HASH, unas claves de **7 dígitos** que nos permitirá identificar los commit y volver a ellos.

    git reflog --hard HEAD <clave>

### ¿Podemos añadir seguridad de alguna forma a nuestro repositorio remoto?

Nuestro repositorio remoto podemos ponerlo público o privado.

Para hacerlo público o privado realizamos lo siguiente:

1. Vaya al panel de proyecto que quiera convertir en público o privado.

2. En el lado superior derecho de la instancia de proyecto clásico, haz clic en  **Menú**.

3. Haga clic en los **3 puntitos** y después en Configuración.

4. En **Visibilidad**, elija la conversión del panel de proyecto en público o privado.

5. Pulsamos sobre **Guardar**.


También podemos dar permisos para poder elegir quien puede realizar cambios en nuestro proyecto.

Para dar permisos deberemos realizar lo siguiente:

1. Nos metemos en el **repositorio**.
2. Seleccionamos la opcion **ajustes**.
3. Accedemos a **collaborators**.
4. Pulsamos sobre **añadir personas**.

Esa persona ya podrá realizar cambios.

Podemos crear reglas para proteger el repositorio:
- **Restricciones de creaciones**.
- **Restricciones de actualizaciones**.
- **Restricciones de borrados**.
- **Requerir historial**.
- **Requerir la firma en los commits**.
- **Requerir una pull request antes de realizar un merge**.
- **Bloquear push forzados.**




# Parte 3 

### ¿Qué es una Pull Request? ¿Cómo podriamos realizar una? ¿Qué utilidad tiene?



### Conflictos que nos han surgido.


