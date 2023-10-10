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

```code

```
</details>

- __git commit -m "añadido fichero .gitignore"__
<details>
<summary>salida</summary>

```code

```
</details>

> __Pregunta2:__ 


</div>
