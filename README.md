Creación de repositorio y archivos:

mkdir practica_evaluable
cd practica_evaluable
git init
Creación y validación de archivos:

touch documento1.txt documento2.txt
Añadir texto a ambos archivos.
git add documento1.txt documento2.txt
git commit -m "Añadidos documento1.txt y documento2.txt"
Realizar cambios en documento1.txt:

Realizar cambios en documento1.txt
git add documento1.txt
git commit -m "Cambios en documento1.txt"
Realizar cambios en documento2.txt y revertirlos:

Realizar cambios en documento2.txt
git add documento2.txt
git commit -m "Cambios en documento2.txt"
git reset --hard HEAD~1
Crear y validar documento3.txt:

touch documento3.txt
Añadir contenido a documento3.txt.
git add documento3.txt
git commit -m "Añadido documento3.txt"
Revertir el último commit:

git revert HEAD
Seleccionar mensaje y cerrar el editor.
Conectar con repositorio remoto:

git remote add origin <URL_del_repositorio>
git push -u origin main
Crear y validar rama mirama:

git checkout -b mirama
Crear y validar rama1.txt y rama2.txt.
git add rama1.txt rama2.txt
git commit -m "Añadidos rama1.txt y rama2.txt en mirama"
Fusionar rama mirama con main:

git checkout main
git merge mirama
git branch -d mirama
Sincronizar con repositorio remoto:

git push origin main
Crear etiqueta V1 y subirla al remoto:

git tag V1
git push origin V1
Clonar repositorio remoto en practica_evaluable_2:

git clone <URL_del_repositorio> practica_evaluable_2
Crear y validar rama mirama en practica_evaluable_2:

cd practica_evaluable_2
git checkout -b mirama
Realizar cambios en documento1.txt.
git add documento1.txt
git commit -m "Cambios en documento1.txt"
Realizar cambios en main de documento2.txt y subirlos al remoto:

Realizar cambios en documento2.txt.
git add documento2.txt
git commit -m "Cambios en documento2.txt"
git push origin main
Merge de ramas y eliminación de mirama:

git checkout main
git merge mirama
git branch -d mirama
git push origin main
Realizar cambios en documento2.txt:

Realizar cambios en documento2.txt.
git add documento2.txt
git commit -m "Cambios en documento2.txt"
Crear y validar rama mirama y realizar cambios distintos en documento2.txt:

git checkout -b mirama
Realizar cambios distintos en documento2.txt.
git add documento2.txt
git commit -m "Cambios distintos en documento2.txt"
Fusionar ramas y resolver conflicto:

git checkout main
git merge mirama
Resolver conflicto.
git add documento2.txt
git commit -m "Resolución de conflicto"
Sincronizar con repositorio remoto:

git push origin main
Añadir README.md al repositorio remoto:

Crear README.md y añadir descripción y comandos.
git add README.md
git commit -m "Añadido README.md"
git push origin main
Sincronizar con repositorio local:

git pull origin main
