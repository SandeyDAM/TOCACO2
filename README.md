# TOCACO2
Trabajo sobre documentación de gestión de repositorios o algo así

## Trabajo realizado por Javier Cotillas, Alejandro Costa, Domingo Cabrero y Angél Toledo

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
  
### ¿Qué es el fichero .gitignore?

Gitignore es una herramienta utilizada en Git para excluir archivos y directorios del control de versiones. Ayuda a los usuarios a mantener sus repositorios limpios y organizados evitando que se rastreen archivos innecesarios.

Consiste en un archivo de configuración que contiene una lista de patrones donde se especifican archivos o directorios que Git debe ignorar.
Sigue una sintaxis en la que los patrones pueden incluir comodines (*), negación (/) y comentarios (#). Dependiendo de su ubicación en el proyecto, los archivos Gitignore pueden ser locales, globales o a nivel de repositorio.

Para crear estos archivos, basta con crear un archivo de texto plano con el nombre .gitignore en el directorio root de tu repositorio Git.

Acto seguido, los usuarios podrán especificar los archivos o directorios que deseen ignorar utilizando patrones Gitignore. Por ejemplo, para ignorar todos los archivos .txt en un directorio llamado price_list, puedes crear un archivo Gitignore con el siguiente contenido:

    *.txt 
    price_list/


