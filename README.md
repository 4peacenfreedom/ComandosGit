
# Guía Básica de Comandos de Git

Git es un sistema de control de versiones distribuido que permite a los desarrolladores trabajar en proyectos de manera colaborativa. A continuación se presenta una lista de comandos básicos para empezar a trabajar con Git.

## Configuración Inicial

Antes de comenzar a usar Git, es importante configurar tu nombre de usuario y correo electrónico:

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tuemail@example.com"
Comandos Básicos
1. Inicializar un Repositorio
Para crear un nuevo repositorio de Git en tu directorio actual:

bash
Copiar código
git init
2. Clonar un Repositorio
Para clonar un repositorio remoto en tu máquina local:

bash
Copiar código
git clone https://github.com/usuario/repositorio.git
3. Ver el Estado del Repositorio
Para ver el estado actual de tu repositorio, incluyendo cambios no guardados y archivos no rastreados:

bash
Copiar código
git status
4. Añadir Archivos al Área de Staging
Para añadir archivos específicos al área de staging:

bash
Copiar código
git add nombre_archivo
Para añadir todos los archivos al área de staging:

bash
Copiar código
git add .
5. Hacer un Commit
Para guardar los cambios en el repositorio:

bash
Copiar código
git commit -m "Mensaje del commit"
6. Ver el Historial de Commits
Para ver el historial de commits del repositorio:

bash
Copiar código
git log
7. Crear una Nueva Rama
Para crear una nueva rama:

bash
Copiar código
git branch nombre_rama
Para cambiar a una rama existente:

bash
Copiar código
git checkout nombre_rama
Para crear y cambiar a una nueva rama en un solo comando:

bash
Copiar código
git checkout -b nombre_rama
8. Fusionar Ramas
Para fusionar una rama en la rama actual:

bash
Copiar código
git merge nombre_rama
9. Eliminar una Rama
Para eliminar una rama que ya no necesitas:

bash
Copiar código
git branch -d nombre_rama
10. Actualizar y Fusionar Cambios del Repositorio Remoto
Para obtener los últimos cambios del repositorio remoto y fusionarlos en la rama actual:

bash
Copiar código
git pull
11. Enviar Cambios al Repositorio Remoto
Para enviar tus commits locales al repositorio remoto:

bash
Copiar código
git push origin nombre_rama
Comandos Adicionales
Descartar Cambios en Archivos
Para descartar cambios en un archivo específico:

bash
Copiar código
git checkout -- nombre_archivo
Restablecer el Área de Staging
Para quitar todos los archivos del área de staging (manteniéndolos en el directorio de trabajo):

bash
Copiar código
git reset
Restablecer un Commit Anterior
Para restablecer el repositorio a un commit anterior (destruyendo cambios posteriores):

bash
Copiar código
git reset --hard id_commit
