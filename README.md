# Git

> Este es un pequelo manual de los comando que mas usamos en git

## Pasos para inicializar un proyecto nuevo
- Creamos el repositorio remoto en GitHub.
- Si no tenemos creado un carpeta en nuestra maquina la creamos y la abrimos con `Visual Studio Code`.
- Si ya tenemos creada la carpeta simplemente la abrimos con `Visual Studio Code`.
- En Abrimos un terminal integrada en `VS Code(Visual Studio Code)`.
- Escribimos lo siguiente para inicializar el repositorio local:
``` shell
git init
```
- Despues hacemos lo siguiente para renombrar el branch por defecto que es `master` a `main`(Ojo que un repositorio solo debe tener o master o main, no ambos):
``` shell
git branch -M main
```
- Si es un proyecto de `Node.js` creamos un archivo llamado `.gitignore`  en el cual escribimos `node_modules` para que esta carpeta no se suba al repositorio, esto por que no es necesario subirla ya que llega a pesar demasiado y puede traer problemas de conflictos con el tiempo.
- Luego hacemos en la terminal para preparar todos los archivos para la confirmacion(commit):
``` shell
git add .
```
- Despues creamos nuestro primer `commit` con el siguinte comando:
``` shell
git commit -m "first commit"
```
- Despues de crear el commit asociamos el repositorio local con el remoto, para esto debemos ejecutal el siguiente comando, el cual pueden encontrar en `Github` al momento que creamos el repositorio(Remplazar <<URL_REPOSITORIO>> por la url del repositorio remoto):
``` shell
git remote add origin <<URL_REPOSITORIO>>
```
- Si por alguna razon nos quedo mal la url del repositorio podemos ejecutar el siguiente comando para eliminar la asociacion con este comando y despues hacemos el paso anterior:
``` shell
git remote remove origin
```
- Por ultimo subimos el branch `main` al repositorio remoto:
``` shell
git push -u origin main
```

