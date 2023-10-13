<div align="justify">

# my-proyecto-millonario
### Rubén Abreu González

---

## Trabajo diario a través de git
- Crear un repositorio en vuestro GitHub llamado my-proyecto-millonario.
- Clonar vuestro repositio en local.
- git clone __git@github.com:alumno-rabgonzalez/my-proyecto-millonario.git__

---

## README
Crear (si no lo habéis creado ya) en vuestro repositorio local un documento __README.md.__
- __touch README.md__
<details>
<summary>salida</summary>

```
```
</details>

---

## Commit inicial 

Añadir al README.md los comanddos utilizados hasta ahora y hacer un coomit inicial con el mensaje commit inicial.

- __git add .__
- __git commit -m "commit inicial"__
<details>
<summary>salida</summary>

```code
inicial"
[main edf7734] commit inicial
 3 files changed, 42 insertions(+), 1 deletion(-)
 rewrite README.md (100%)
 create mode 100644 images/ej1-ets.png
 create mode 100644 images/ej1.1-ets.png
```
</details>

## Push inicial
Subir los cambios al repositorio remoto
- __git push origin master__
<details>
<summary>salida</summary>

```code
Enumerando objetos: 8, listo.
Contando objetos: 100% (8/8), listo.
Compresión delta usando hasta 4 hilos
Comprimiendo objetos: 100% (6/6), listo.
Escribiendo objetos: 100% (6/6), 219.09 KiB | 19.92 MiB/s, listo.
Total 6 (delta 0), reusados 0 (delta 0), pack-reusados 0
To https://github.com/rabgonzalez/my-proyecto-millonario
   d9f4220..edf7734  main -> main
```
</details>

> __Pregunta1:__ Ya que yo he clonado el repositorio de github al repositorio local, no es necesario seleccionar la rama a la que quiero subir los cambios.

## Ignorar archivos
- Crear en el repositorio local un fichero llamado ___privado.txt.___
- __touch privado.txt__
<details>
<summary>salida</summary>

```
```
</details>

- Crear en el repositorio local una carpeta llamada privada.
- __mkdir privada__
<details>
<summary>salida</summary>

```
```
</details>

- Realizar los cambios oportunos para que tanto el archivo como la carpeta sean ignorados por git.
- __echo "privado.txt" >> .gitignore__
<details>
<summary>salida</summary>

```
```
</details>

- __echo "/privada" >> .gitignore__
<details>
<summary>salida</summary>

```
```
</details>

- __git add .__
<details>
<summary>salida</summary>

```
```
</details>

- __git commit -m "añadido fichero .gitignore"__
<details>
<summary>salida</summary>

```code
[main af95674] añadido fichero .gitignore
 4 files changed, 95 insertions(+), 12 deletions(-)
 create mode 100644 .gitignore
 delete mode 100644 images/ej1-ets.png
 delete mode 100644 images/ej1.1-ets.png
```
</details>

> __Pregunta2:__ Los ficheros y directorios que han sido añadidos a .gitignore avisan a git de que deben de ser ignorados a la hora de subirlos al repositorio en la nube

## Añadir fichero 1.txt
- Añadir fichero 1.txt al repositorio local.
- __touch 1.txt__
<details>
<summary>salida</summary>

```
```
</details>

- __git add .__
<details>
<summary>salida</summary>

```
```
</details>

- __git commit -m "añadido 1.txt"__
<details>
<summary>salida</summary>

```code
[main 85d97f7] añadido 1.txt
 2 files changed, 34 insertions(+), 2 deletions(-)
 create mode 100644 1.txt
```
</details>

> __Pregunta3:__ La acción ___git add___ prepara todos los cambios dados en un fichero (git add nombre_fichero) para subirlos a la nube, y ___git commit___ crea un registro que anuncia los cambios que se han dado.

## Crear el tag v0.1
- 1. Crear un tag v0.1
<details>
<summary>salida</summary>

```
```
</details> 

## Subir el tag v0.1
<details>
<summary>salida</summary>

```code
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
 To https://github.com/rabgonzalez/my-proyecto-millonario
 * [new tag]         v0.1 -> v0.1
```
</details> 

> __Pregunta4:__ un tag es un historial de cambios que se almacenan en versiones para poder gestionar su cronología de forma más sencilla.

## Crear una rama v0.2
- Crear una rama v0.2.
- git branch v0.2
<details>
<summary>salida</summary>
```
```
</details>

- Posiciona tu carpeta de trabajo en esta rama.
- git checkout v0.2
<details>
<summary>salida</summary>
```code
Switched to branch 'v0.2'
M       README.md
```
</details>

## Añadir fichero 2.txt
- Añadir un fichero 2.txt en la rama v0.2.
- touch 2.txt
<details>
<summary>salida</summary>
```
```
</details>

> Nota: en windows utilize el comando echo . > 2.txt 

- git add .
<details>
<summary>salida</summary>
```
```
</details>

- git commit -m "añadido 2.txt"
<details>
<summary>salida</summary>
```code
[v0.2 5f3a0e6] añadido 2.txt
 2 files changed, 66 insertions(+)
 create mode 100644 2.txt
```
</details>

> __Pregunta5:__ Crear distintas ramas es útil para hacer pruebas de nuestro código sin modificar la version original (rama main/master) o para no subir al repositorio remoto ciertos cambios, de modo que si estas ramas funcionan podemos usar un ___git merge___ y traerlas a nuestra rama principal. O si no funcionan puedes usar un ___git branch -D___ para borrar la rama. 

## Crear rama remota v0.2
- 1. Subir los cambios al reposiorio remoto.
- git push origin v0.2
<details>
<summary>salida</summary>
```code
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 20 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 843 bytes | 843.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'v0.2' on GitHub by visiting:
remote:      https://github.com/rabgonzalez/my-proyecto-millonario/pull/new/v0.2
remote:
To https://github.com/rabgonzalez/my-proyecto-millonario
 * [new branch]      v0.2 -> v0.2
```
</details>

## Merge directo
- 1. Posicionarse en la rama master/main según sea tu rama principal.
- git checkout master
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

- 1. Hacer un merge de la rama v0.2 en la rama master/main.
- git merge v0.2 -m "merge v0.2 sin conflictos"
<details>
<summary>salida</summary>
```code
 Updating c307e1b..f6720c6
 Fast-forward (no commit created; -m option ignored)
 2.txt     | Bin 0 -> 8 bytes
 README.md | 101 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 2 files changed, 101 insertions(+)
 create mode 100644 2.txt
```
</details> 

> __Pregunta6:__ No se debría de haber producido ningún conflicto ya que la información de ambas ramas ha sido actualizada y guardada, de modo que al hacer el comando ___git merge___ no se va a perder información.

## Merge con conflicto
- 1. En la rama maste/main poner Hola en el fichero 1.txt y hacer commit.
- git checkout master
<details>
<summary>salida</summary>
```code
Already on 'main'
M       README.md
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)
```
</details>

- echo "Hola" >> 1.txt
<details>
<summary>salida</summary>
```
```
</details>

- git add .
<details>
<summary>salida</summary>
```code
```
</details>

- git commit -m "hola en 1.txt"
<details>
<summary>salida</summary>
```code
```
</details>

- 1. Posicionarse en la rama v0.2 y poner Adios en el fichero "1.txt" y hacer commit.
- git checkout v0.2
<details>
<summary>salida</summary>
```code
```
</details>

- echo "Adios" >> 1.txt
<details>
<summary>salida</summary>
```code
```
</details>

- git add .
<details>
<summary>salida</summary>
```code
```
</details>

- git commit -m "adios en 1.txt"
<details>
<summary>salida</summary>
```code
```
</details>

- 1. Posicionarse de nuevo en la rama master/main y hacer un merge con la rama v0.2
- git checkout master
<details>
<summary>salida</summary>
```code
```
</details>

- git merge v0.2
<details>
<summary>salida</summary>
```code
```
</details>

- vim 1.txt
<details>
<summary>salida</summary>
```code
```
</details>

- git add .
<details>
<summary>salida</summary>
```code
```
</details>

- git commit -m "arreglado merge en 1.txt"
<details>
<summary>salida</summary>
```code
```
</details>


</div>
