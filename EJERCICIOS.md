# Ejercicios Parte 2 - Git


### Comandos ejecutados:
```bash
git add notas.md
git commit -m "feat: añade notas iniciales"
git push origin main

# Luego añadí más asignaturas
git commit -am "feat: amplía notas.md"
git push origin main

git checkout -b feature-tareas
# Edición de notas.md para añadir tareas
git add notas.md
git commit -m "feat: añade tareas pendientes"
git push -u origin feature-tareas


echo "contenido temporal" > temporal.txt
git add temporal.txt
git commit -m "chore: añade archivo temporal"
git rm temporal.txt
git commit -m "chore: elimina archivo temporal"
git push

# Intento de restauración (falló)
git restore temporal.txt


git add notas.md
git commit -m "feat: añade Historia"
git add notas.md
git commit -m "feat: añade Filosofía"

git log --oneline --graph --all
git diff HEAD~1 HEAD
