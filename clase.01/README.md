# Clase 01

## Extensiones visual studio code

* GitLens
* Git Graph
* Material Icon Theme

## Verificar que tengo instaldo GIT
```sh
git --version # git -v
```

## Configurar el nombre y el mail para poder realizar commits (fotos)

```sh
git config --global user.name "Maximiliano Principe"
git config --global user.email "mlapeducacionit@gmail.com"
```

## Para saber si tengo todo configurado

```sh
git config --global --get-regexp user
```

## Para quitar alguna propiedad dentro del config

```sh
git config --global --unset user.email
```

## Para inicializar un repositorio de GIT
Esto me crea el repositorio de git. Se crea una carpeta .git (oculta)

```sh
git init
```

## Para saber el estado de los archivos

```sh
git status
```

## Areas posibles en las que pueden estar los archivos

* Working Directory (Directo de trabajo) donde van agregando, borrando al archivo el desarrolllo

* Staging Area (Area de control de cambios) Se agregan los archivos para darle seguimiento y posteriormente sacarles una foto (commit)

* Local Repo (Area de validación de cambios, donde se registran las modificaciones realizadas) Donde van a estar todas las fotos (commit) que vaya sacando.


## Estados de los archivos

* Untracked (Sin seguimiento) => archivos que no se agregaron al index/stage y por consecuente no se les da seguimiento.
* Staged => Archivos que fueron agregados al index/stage area y cuyos cambios van a ser incorporados al repositorio
* Unmodified => Archivos que se cuentran en en el respositorio y no fueron modificado (Con respecto al repositorio)
* Modified => Archivos que se encuentro en el repositorio pero difieren con lo que se encuentra actualmente en el directorio trabajo (Working directory)

## Para pasar un archivo del WK al SA

```sh
git add <nombre-archivo>
git add clase.01/README.md
```

## Para pasar del SA al LR

```sh
git commit -m "<mensaje descriptivo del contenido del commit>"
git commit -m "Esto es mi primer commit"
```

## Para ver la diferencia entre el WD y el LR

```sh
git diff # Para salir del comando si la consola se queda bloqueada (tomada) es presionar la tecla q (quit)
```

## Para ver las fotos dentro de la caja de fotos 

```sh
git log # Forma larga
git log --oneline # Forma corta
```



