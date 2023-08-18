# Clase 03

# GIT MERGE
Para fusionar las ramas tengo que utilizar el comando **git merge**

*IMPORTANTE*: Tengo que estar en la rama destino de los cambios que QUIERO traerme (main).
EJ: Si quiero traerme tarea footer al main, tendria que hacer

```sh
git merge <rama-que-quiero-traerme>
git merge tarea-footer
```
# En caso de que hayan conflictos
* Si no estan disponibles los integrantes del equipo que estuvieron trabajando, tengo que abortar la fusion
```sh
git merge --abort
```
## Tipos de fusiones

* Fast-fowards => (No hay ningun conflicto, se hace de manera automatica)
* Recursivo => (No hay ningun conflicto, se hace de manera automatica)
* Manual => (Conflictos - Vamos a tener que resolverlos manualmente. Para indicarle a git que lo resolvimos, hay que hacer un commit)

## GIT STASH
Permite registrar temporalmente los cambios que aun no fueron commiteados (guardados dentro del repo) (Cambios que estan en el Working Directory o en SA) para guardarlos dentro de un area temporal para seguir trabajando luego. *Los stashes se guardan localmente*.

```sh
git stash
```

### Crear un stash
```sh
git stash
```

### Listar los stash
```sh
git stash list
```

### Sacar el elemento que esta en el stash
```sh
git stash pop
```

## Para eliminar un stash

```sh
git stash drop # Va a borrar el ultimo stash
git stash drop stash@{2} # Va a borrar el indicado
```

## Aplico un stash en particular y no borro el stash
```sh
git stash apply # Va a desapilar el primero de la pila
git stash apply stash@{5} # Me desapila el stash 5
```

> NO BORRA EL STASH recuperado

## Puedo a partir de un stash crear una rama
```sh
git stash branch <nombre-de-la-rama>
git stash branch rama-stash # Saca del stash lo que este dentro y lo pone en una nueva rama
```


