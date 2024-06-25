
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
```bash
git init
```

# Clonar un repositorio existente
```bash
git clone https://github.com/usuario/repositorio.git
```
# Ver el estado del repositorio
```bash
git status
```
# Agregar archivos al área de preparación
```bash
git add nombre_del_archivo
git add .
```
# Confirmar cambios en el repositorio
```bash
git commit -m "Mensaje de confirmación"
```
## Trabajando con Ramas
# Listar ramas existentes
```bash
git branch
```
# Crear una nueva rama
```bash
git branch nombre_de_la_rama
```
# Cambiar a una rama específica
```bash
git checkout nombre_de_la_rama
```
# Crear y cambiar a una nueva rama
```bash
git checkout -b nombre_de_la_rama
```
# Fusionar una rama con la rama actual
```bash
git merge nombre_de_la_rama
```
## Remotos
# Ver los repositorios remotos
```bash
git remote -v
```
# Agregar un repositorio remoto
```bash
git remote add origin https://github.com/usuario/repositorio.git
```
# Obtener cambios del repositorio remoto
```bash
git pull origin main
```
## Deshacer Cambios


# Enviar cambios al repositorio remoto
```bash
git push origin main
```
## Deshacer Cambios

# Deshacer cambios en el área de trabajo
```bash
git checkout -- nombre_del_archivo
```
# Restablecer el área de preparación
```bash
git reset nombre_del_archivo
```
# Deshacer una confirmación específica
```bash
git revert id_de_confirmación
```
# Restablecer el repositorio a un estado anterior
```bash
git reset --hard id_de_confirmación
```
# Importante : 
Verificar los commits recientes:
```bash
git log

git reset --hard HEAD~Camtodad de commit a eliminar
Por ejemplo, para eliminar los últimos 3 commits, usarías:


git reset --hard HEAD~3
git push origin nombre-de-la-rama --force

```


## Otros Comandos Útiles
# Mostrar diferencias entre archivos
```bash
git diff
```
# Guardar cambios temporalmente
```bash
git stash
```
# Aplicar cambios guardados temporalmente
```bash
git stash pop
```
# Ver registros de stashes
```bash
git stash list
```

# Ver el historial de confirmaciones
```bash
git log
```
