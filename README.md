# Comandos esenciales de GIT

Guía de referencia con los comandos más utilizados en git.

---

RESUMEN (MAS UTILIZADOS)

| Comando | Uso |
|---|---|
| `git status` | Revisar cambios |
| `git pull` | Actualizar proyecto |
| `git switch` | Cambiar rama |
| `git add` | Preparar cambios |
| `git commit` | Guardar cambios |
| `git push` | Subir código |
| `git diff` | Revisar modificaciones |
| `git log` | Revisar historial |
| `git stash` | Guardar cambios temporales |
| `git restore` | Deshacer cambios |


---

#  Git

Permiten trabajar en equipo, guardar cambios, crear ramas y administrar versiones del código.

---

## Ver estado del proyecto

```bash
git status
```

Muestra:

- Archivos modificados
- Archivos nuevos
- Archivos eliminados
- Rama actual
- Cambios pendientes de guardar

Uso diario antes de realizar cualquier operación.

---

## Agregar archivos al staging

```bash
git add archivo.java
```

Agrega un archivo específico para preparar un commit.

Ejemplo:

```bash
git add CuentaBancaria.java
```

---

## Agregar todos los cambios

```bash
git add .
```

Agrega todos los archivos modificados del proyecto.

---

## Crear un commit

```bash
git commit -m "mensaje"
```

Guarda los cambios con una descripción.

Ejemplo:

```bash
git commit -m "feat: agregar validacion de transferencia"
```

---

## Enviar cambios al repositorio remoto

```bash
git push
```

Sube los commits al servidor:

- GitHub
- GitLab
- Bitbucket

---

## Descargar cambios del equipo

```bash
git pull
```

Obtiene cambios del repositorio remoto y los integra.

Uso común:

```bash
git pull origin main
```

---

## Descargar cambios sin mezclar

```bash
git fetch
```

Descarga información del remoto pero no modifica tu código.

---

## Crear una rama

```bash
git branch nombre-rama
```

Ejemplo:

```bash
git branch feature/login
```

---

## Crear y cambiar de rama

```bash
git switch -c nombre-rama
```

Ejemplo:

```bash
git switch -c feature/pagos
```

---

## Cambiar de rama

```bash
git switch nombre-rama
```

Ejemplo:

```bash
git switch main
```

---

## Ver ramas disponibles

```bash
git branch
```

Muestra las ramas locales.

---

## Fusionar ramas

```bash
git merge nombre-rama
```

Une cambios de otra rama con la actual.

Ejemplo:

```bash
git merge feature/login
```

---

## Ver historial de commits

```bash
git log --oneline --graph --all
```

Muestra:

- Historial
- Ramas
- Relaciones entre commits

---

## Ver diferencias

```bash
git diff
```

Muestra cambios línea por línea antes de hacer commit.

---

## Guardar cambios temporalmente

```bash
git stash
```

Guarda cambios actuales sin crear commit.

Útil cuando necesitas cambiar de tarea rápidamente.

---

## Recuperar cambios guardados

```bash
git stash pop
```

Restaura los cambios almacenados.

---

## Deshacer cambios de un archivo

```bash
git restore archivo
```

Elimina cambios no guardados.

Ejemplo:

```bash
git restore Main.java
```

---

## Revertir un commit

```bash
git revert HASH
```

Crea un nuevo commit que deshace otro.

Muy utilizado en producción.

---

## Copiar un commit específico

```bash
git cherry-pick HASH
```

Aplica un commit específico en otra rama.

---

