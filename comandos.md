Pasos típicos para guardar cambios y subirlos
(La forma común desde la terminal):

git add .
git push
git commit -m "mensaje del commit"

git add . → prepara los archivos para el commit

git commit → guarda los cambios

git push → sube los cambios a GitHub

Agregar solo un archivo

También es posible añadir un archivo específico, con:

git add archivo.txt
git commit -m "cambio en archivo"
git push

Comandos adicionales(del profesor):

git clone <url-del-repositorio>: Clonar repositorio

gh repo clone <repositorio>: Clonar repositorio con GitHub CLI

gh auth login: Se loguea a github de forma semi automatica.

git add <[archivo...]>: Agrega archivos a la etapa de staging.

git status: Da el estado del repositorio.

git push: Publica en la nube los ultimos commit.

git pull: Descarga de la nube los ultimos commit.
