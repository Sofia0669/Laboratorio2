# Inicializar repositorio
git init

# Cambiar nombre de la rama principal
git branch -M main

# Primer commit
git add .
git commit -m "Estructura inicial del proyecto"

# Ver historial
git log --oneline

# Crear y cambiar a rama desarrollo
git checkout -b desarrollo

# Commit en desarrollo
git add .
git commit -m "Agrega contenido en index"

# Volver a main
git checkout main

# Merge de ramas
git merge desarrollo

# Modificar styles.css SIN commit
git diff

# Commit temporal
git add .
git commit -m "Cambio temporal"

# Eliminar último commit
git reset --hard HEAD~1

# Ver historial completo
git reflog

# Recuperar commit eliminado
git reset --hard 984530c

# Crear .gitignore 
New-Item .gitignore

# Commit gitignore
git add .
git commit -m "Agrega gitignore"

# Vincular repositorio
git remote add origin https://github.com/Sofia0669/Laboratorio2.git
# Subir proyecto
git push -u origin main

# Crear rama login
git checkout -b login

# Crear archivo login
New-Item login.html

# Commit login
git add .
git commit -m "Agrega login"

# Subir rama login
git push origin login