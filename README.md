# Ejercicio 1
### ¿Cómo podrías pausar el trabajo en el commit actual para dedicarte a trabajar en master?

Con el comando **git stash**, que guarda en el Stage los archivos modificados y que no han sido confirmados.
Luego, los saco del Stage con **git stash pop** y retomo el trabajo.

```
git stash
git checkout main
rm status.js
git add .
git commit -m "elimina status.js"
git push
git checkout custom-navbar
git stash pop
```







# Ejercicio 2
### ¿Cómo podrías subir los cambios a producción si es la rama master la que se usa para producción?

Con un pull request desde GitHub. Cuando se valida el codigo, se fusiona la rama (merge)
