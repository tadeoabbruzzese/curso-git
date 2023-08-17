## Clase 02

## ADD: Otras formas de colocar en el staging area los archivos

```sh
git add -p # git add --patch
```

* y:  agregar el hunk (trocito de código) al stage (staging area)
* s:  dividir el hunk en varios (automatico)
* n:  descarta ese hunk
* e:  editar manualmente el hunk (Tengo que comentar la línea que no quiero que pase al SA)
* ?:  ayuda

# CLONE: Me permite clonar el repositorio (Completo con la historia de fotos)

```sh
git clone <url-del-repo>
git clone https://github.com/twbs/bootstrap.git . # Punto (.) Le digo no crees una carpeta, bajalo en el directorio (carpeta) sin crear una
```

# .gitignore: Me permite descargar archivos que no quiero que formen parte del repositorio.
Para eso tengo que crear en general un archivo nuevo llamado '.gitignore' y colocarle el nombre o carpeta a ignorar.

# AMEND: Me permite enmendar un commit.
Arreglar el mensaje del commit o agregar archivos o partes de una archivo que me quedaron fuera del commit.

```sh
git commit --amend -m "Nuevo mensaje"
```

## gitkeep: Me permite seguir carpetas vacías.
Git no versiona carpetas. Si yo quisiera que git siga una carpeta tengo que crear un archivo llamado por la comunidad. **.gitkeep**

## REMOTE: Me permite agregar la URL del repositorio em el local para luego subir los cambios

```sh
git remote 
git remote -v #informacion detallada
```