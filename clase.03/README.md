# Clase 03

# GIT MERGE
Para fusionar las ramas tengo que utilizar el comando **git merge**

*IMPORTANTE:* Tengo que estar en la rama destino de los cambios que QUIERO traerme (main).
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
