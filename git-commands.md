# Git - Comandos Más Importantes

## Configuración inicial

Ver configuración actual:

```bash
git config --list
```

Configurar nombre de usuario:

```bash
git config --global user.name "Tu Nombre"
```

Configurar correo electrónico:

```bash
git config --global user.email "correo@ejemplo.com"
```

---

## Crear y clonar repositorios

Inicializar un repositorio:

```bash
git init
```

Clonar un repositorio:

```bash
git clone https://github.com/usuario/repositorio.git
```

Clonar una rama específica:

```bash
git clone -b rama https://github.com/usuario/repositorio.git
```

---

## Estado y seguimiento

Ver estado de los archivos:

```bash
git status
```

Ver historial resumido:

```bash
git log --oneline
```

Ver historial gráfico:

```bash
git log --oneline --graph --decorate --all
```

Ver diferencias:

```bash
git diff
```

---

## Agregar cambios

Agregar un archivo:

```bash
git add archivo.txt
```

Agregar todos los cambios:

```bash
git add .
```

---

## Commits

Crear commit:

```bash
git commit -m "Descripción de cambios"
```

Agregar y hacer commit en un solo paso:

```bash
git commit -am "Descripción de cambios"
```

Modificar el último commit:

```bash
git commit --amend
```

---

## Ramas

Listar ramas:

```bash
git branch
```

Crear una nueva rama:

```bash
git branch feature/nueva-funcionalidad
```

Cambiar de rama:

```bash
git switch nombre-rama
```

Crear y cambiar a una rama:

```bash
git switch -c feature/nueva-funcionalidad
```

Eliminar una rama local:

```bash
git branch -d nombre-rama
```

---

## Trabajo con repositorios remotos

Ver repositorios remotos:

```bash
git remote -v
```

Agregar repositorio remoto:

```bash
git remote add origin https://github.com/usuario/repositorio.git
```

Enviar cambios:

```bash
git push origin main
```

Enviar una nueva rama:

```bash
git push -u origin feature/nueva-funcionalidad
```

Obtener cambios:

```bash
git pull
```

Descargar cambios sin fusionar:

```bash
git fetch
```

---

## Merge y Rebase

Fusionar una rama:

```bash
git merge nombre-rama
```

Rebase:

```bash
git rebase main
```

Abortar rebase:

```bash
git rebase --abort
```

---

## Deshacer cambios

Descartar cambios locales:

```bash
git restore archivo.txt
```

Eliminar archivos del área de staging:

```bash
git restore --staged archivo.txt
```

Volver a un commit específico:

```bash
git reset --hard <commit-id>
```

Revertir un commit:

```bash
git revert <commit-id>
```

---

## Stash

Guardar cambios temporales:

```bash
git stash
```

Ver stashes:

```bash
git stash list
```

Recuperar último stash:

```bash
git stash pop
```

---

## Etiquetas (Tags)

Crear tag:

```bash
git tag v1.0.0
```

Enviar tags al remoto:

```bash
git push origin --tags
```

Listar tags:

```bash
git tag
```

---

## Limpieza

Eliminar archivos no versionados:

```bash
git clean -fd
```

Ver qué se eliminaría:

```bash
git clean -fdn
```

---

## Comandos útiles para GitHub

Agregar repositorio remoto:

```bash
git remote add origin https://github.com/usuario/repositorio.git
```

Primer push:

```bash
git push -u origin main
```

Actualizar rama local:

```bash
git pull origin main
```

---

## Flujo de trabajo básico

```bash
git pull
git checkout
