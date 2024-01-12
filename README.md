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

     $ git clone https://github.com/UC3Music-e/test-repository.git

Este mediante protocolo HTTP.

    $ git clone git@github.com:UC3Music-e/test-repository.git

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

### Proceso de merge entre ramas.


### Resolución de conflictos en un merge


### Diferencias entre un pull y un fetch.


### ¿Cómo podríamos volver a una versión anterior del proyecto?


### ¿Podemos añadir seguridad de alguna forma a nuestro repositorio remoto?


