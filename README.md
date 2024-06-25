
## Guía Básica de Comandos de Git

Git es un sistema de control de versiones distribuido que permite a los desarrolladores trabajar en proyectos de manera colaborativa. A continuación se presenta una lista de comandos básicos para empezar a trabajar con Git.

## Configuración Inicial

Antes de comenzar a usar Git, es importante configurar tu nombre de usuario y correo electrónico:


```bash
# Configurar nombre de usuario
git config --global user.name "Tu Nombre"

# Configurar correo electrónico
git config --global user.email "tuemail@example.com"
```
## Comandos Básicos
# Crear un nuevo repositorio
git init

# Clonar un repositorio existente
git clone https://github.com/usuario/repositorio.git

# Ver el estado del repositorio
git status

# Agregar archivos al área de preparación
git add nombre_del_archivo
git add .

# Confirmar cambios en el repositorio
git commit -m "Mensaje de confirmación"

## Trabajando con Ramas
# Listar ramas existentes
git branch

# Crear una nueva rama
git branch nombre_de_la_rama

# Cambiar a una rama específica
git checkout nombre_de_la_rama

# Crear y cambiar a una nueva rama
git checkout -b nombre_de_la_rama

# Fusionar una rama con la rama actual
git merge nombre_de_la_rama

## Remotos
# Ver los repositorios remotos
git remote -v

# Agregar un repositorio remoto
git remote add origin https://github.com/usuario/repositorio.git

# Obtener cambios del repositorio remoto
git pull origin main
## Deshacer Cambios


# Enviar cambios al repositorio remoto
git push origin main

## Deshacer Cambios

# Deshacer cambios en el área de trabajo
git checkout -- nombre_del_archivo

# Restablecer el área de preparación
git reset nombre_del_archivo

# Deshacer una confirmación específica
git revert id_de_confirmación

# Restablecer el repositorio a un estado anterior
git reset --hard id_de_confirmación

## Otros Comandos Útiles
# Mostrar diferencias entre archivos
git diff

# Guardar cambios temporalmente
git stash

# Aplicar cambios guardados temporalmente
git stash pop

# Ver registros de stashes
git stash list


# Ver el historial de confirmaciones
git log
