# Sesiones

## Sesion 1 


## Sesion 2 


## Sesion 3

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

Existen otros comandos si queremos ser mas expecificos, al momento de agregar archivos al commit. Por ejemplo, si queremos agregar solamente un archivo index.html

```sh
$ git add "index.html"
```


Si queremos retirar algun archivo de nuestro **staging** area. Usaremos el siguiente comando

```sh
$ git restore --staged <file>
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

El comando git commit toma todos los contenidos de los archivos a los que se les realiza el seguimiento con **git add** y registra una nueva instantánea permanente en la base de datos y luego avanza el puntero de la rama en la rama actual.

Si no colocamos **-m** nos abrir nuestro editor de texto predeterminado para agregar el comentario.

```sh
$ git commit -m "Primer Commit"
```

<p align="center">
  <img src="/img/gitcommitcommand.JPG" alt="git commit" >
</p>
