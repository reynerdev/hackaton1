# Sesiones
[![](https://img.shields.io/badge/badge-Alumno%20Reyner%20Loza-blue)](https://www.instagram.com/hreloza/)
## Sesion 1

En esta sesión se explicó todo lo relacioando al *Backend*. Qué es lo que realiza un desarollador BackEnd. Las diferencias con el *FrontEnd*. Las tecnologias que se usan actualmente para el desarollo del *Backend*

Aca tenemos un enlace a una fuente donde nos muestra gráficamente el camino a seguir (Roadmap) para un desarolllador actualizado para esteaño 2020. Todas las tecnologias que un desarollor backend deberia de aprender.
[![](https://img.shields.io/badge/-Shareable%20Link%20-0a0a0a.svg?style=flat&colorA=0a0a0a)](https://roadmap.sh/frontend)

## Sesion 2 

Entender la diferencias entre  un editor de  código  e IDE's y realizar la configuracion correcto de Visual Studio Code.



### IDE

Son herramientas mas complejos que nos brinda varias posibilidades como debugger en tiempo real. Se usa mayormente para proyectos grandes.
<img src="/img/vstudio.jpg" align="right"
     alt="Visual Studio" width="180" height="178">
Utiliza un IDE cuando [(enlace)]:

* El lenguaje de programacion sea compilado, Java por ejemplo, eso de estar compilando cada clase por tu cuenta cuando es un proyecto enorme es un gran problema, deja que un IDE lo haga por ti.
* Estas diseñando una interfaz grafica de usuario, nada mejor que un IDE con un bonito drag and drop, para solo soltar los elementos en el lugar que quieras que salgan.
* Estas aprendiendo un lenguaje nuevo, no sabes la sintaxis, ni los metodos ni nada. La ayuda y completado de codigo del IDE hara tu aprendizaje mas facil y amistoso.
* Tienes una computadora con suficientes recursos.
* Rquiere una licencia 



### Editores de texto
 
Un editor de texto es un herramienta mas simple que se encuentra integrado ya en un IDE, pero en esta oportunidad lo tenemos como una herramienta externa y facil de usar. Ultimamente, exiten varios complementos que estan logrando que un editor de texto sea capaz de imitar algunas de las cualidades de un ide, como la funcion de autocompletado,

 Utilizar editores de texto cuando [(enlace)]:


* Tengas una computadora con muy pocos recursos
* El lenguaje de programación que utilices no sea compilado (php, javascript, ruby, etc)
* Estas creando sitios web estáticos
* Eres experto en el lenguaje que estas programando, tan experto que solo con tener la documentación a la mano es suficiente para hacer maravillas.
* La mayoria son gratis.
* Facil de aprender 
[Enlace]:https://ingeniaoaxaca.com/que-diferencias-hay-entre-un-editor-y-un-ide-a-la-hora-de-escribir-codigo/

Uno de los editores de texto mas usados ultimamente es Visual Studio Code.

<p align="center">
  <img src="/img/vscode.png" alt="git init" width="738">
</p>

## Sesion 3

En este sesión se estudio el software para el manejo de versiones llamado [Git] usando los repositorios de [Git Hub] 

[Git]:https://git-scm.com/ 
[Git Hub]:https://github.com/


### git init

Inicializa el repositorio Git en la carpeta donde se ejecuta el comando

```sh
$ git init
```

<p align="center">
  <img src="/img/gitinit.JPG" alt="git init" width="738">
</p>


### git add . 

Agregamos los archivos para que se encuentren en el **"staging area"** o **index** listos para usar **"commit"**

```sh
$ git add . 
```
<p align="center">
  <img src="/img/gitaddcommand.JPG" alt="git init" width="738">
</p>

Existen otros comandos si queremos ser mas especificos, al momento de agregar archivos al commit. Por ejemplo, si queremos agregar solamente un archivo index.html

```sh
$ git add "index.html"
```


Si queremos retirar algun archivo de nuestro **staging** area. Usaremos el siguiente comando

```sh
$ git restore --staged <file>
```

Otros comandos que se puede utilizar 

* Cuando se quiere agregar un tipo de archivo al **Staging Area** . Por ejemplo, en este caso, queremos agregar los archivos `.html`

```sh
$ git add *.html
```

### git status 

El comando git status te mostrará los diferentes estados de los archivos en tu directorio de trabajo y área de ensayo. Qué archivos están modificados y sin seguimiento y cuáles con seguimiento pero no confirmados aún. En su forma normal, también te mostrará algunos consejos básicos sobre cómo mover archivos entre estas etapa

```sh
$ git status
```

<p align="center">
  <img src="/img/gitstatus.JPG" alt="git init" >
</p>

<p align="center">
  <img src="/img/gitstatusresult.JPG" alt="git status" >
</p>

### git commit

El comando git commit toma todos los contenidos de los archivos a los que se les realiza el seguimiento con `git add` y registra una nueva instantánea permanente en la base de datos y luego avanza el puntero de la rama en la rama actual.

Si no colocamos `-m` nos abrirá nuestro editor de texto predeterminado para agregar el comentario.

```sh
$ git commit -m "Primer Commit"
```

<p align="center">
  <img src="/img/gitcommitcommand.JPG" alt="git commit" >
</p>


## git branch 

Cuando necesitamos crear un branch. Realizaremos el siguiente codigo. Supongamos que nuestro **branch** ( rama) se llame **"Parte2"**

```sh
$ git branch Parte2
```

Ahora, para estar trabajando en nuestra rama. Ejecutamos el siguiente comando. 

```sh
$ git checkout Parte2
```

En este momento si ejecutamos el comando `git status` nos saldra `On branch Parte2`. Quiere decir que estamos en nuestra rama "Parte2". 

Para volver al master solo tenemos que ejecutar el siguiente comando

```sh
$ git checkout master
```

## git push


Para enviar nuestros archivos confirmados a nuestro repositorio que puede ser **GitHub** o **GitLab**. Usaremos el comando `git pull <dirrecion http de nuestro repositorio`. 

Para este repositorio sería

```sh
git push https://github.com/reynerdev/hackaton1.git
```

## git clone

Cuando necesitemos clonar un repositorio , usamos el comando `clone`. Estaremos haciendo una copia del depositorio a nuestra disco duro.

```sh
git clone https://github.com/reynerdev/hackaton1.git
```