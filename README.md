# TOCACO2
Trabajo sobre documentación de gestión de repositorios o algo así

## Trabajo realizado por Javier Cotillas, Alejandro Costa, Domingo Cabrero y Angél Toledo

# Parte 1 

### ¿Cómo podemos crear un repositorio remoto?
    
Para llevar nuestro repositorio local a un repositorio remoto, primero tenemos que crear un repositorio en GitHub que para hacerlo debemos ir al DashBoard de nuestro GitHub y en la parte derecha nos saldrá un + que al darle ahi nos llevará a un menú, donde le pondremos nombre 
 

### ¿Qué es el README.md?

Los archivos readme son archivos que contienen información importante sobre el sistema, proyecto o software al que hacen referencia. Debido a su utilidad, se recomienda ubicarlo en el nivel supeiror del directorio para que sea fácil de encontrar por los usuarios.


### ¿Qué es el fichero .gitignore?

Gitignore es una herramienta utilizada en Git para excluir archivos y directorios del control de versiones. Ayuda a los usuarios a mantener sus repositorios limpios y organizados evitando que se rastreen archivos innecesarios.

Consiste en un archivo de configuración que contiene una lista de patrones donde se especifican archivos o directorios que Git debe ignorar.
Sigue una sintaxis en la que los patrones pueden incluir comodines (*), negación (/) y comentarios (#). Dependiendo de su ubicación en el proyecto, los archivos Gitignore pueden ser locales, globales o a nivel de repositorio.

Para crear estos archivos, basta con crear un archivo de texto plano con el nombre .gitignore en el directorio root de tu repositorio Git.

Acto seguido, los usuarios podrán especificar los archivos o directorios que deseen ignorar utilizando patrones Gitignore. Por ejemplo, para ignorar todos los archivos .txt en un directorio llamado price_list, puedes crear un archivo Gitignore con el siguiente contenido:

*.txt
price_list/
