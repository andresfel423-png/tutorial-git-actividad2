<p align="center"><img src="logo\_uniagraria.png" alt="Logo UNIAGRARIA" width="160"></p>

# Tutorial de Git – Actividad 2: Hands on, configuración de herramientas

**Universidad:** Fundación Universitaria Agraria de Colombia – UNIAGRARIA 
**Curso:** Ciencia de Datos (Profesional)
**Estudiante:** Andres Felipe Amaya Camacho
**Docente:** Carlos Andres Gomez Vasco

## Descripción

Repositorio individual de la Actividad 2. Contiene un tutorial de Git elaborado a partir del libro *Pro Git* (Chacon y Straub, 2.ª ed., https://git-scm.com/book/es/v2): un documento de Word por capítulo, exportado también a PDF. El objetivo es practicar los comandos básicos de Git (`clone`, `add`, `commit`, `push`) y la redacción de mensajes de confirmación claros y descriptivos.

## Herramientas usadas

* **Git** (control de versiones) y **GitHub** (repositorio remoto).
* **Microsoft Word** para redactar los capítulos y exportarlos a PDF.
* **Terminal / Git Bash** para ejecutar los comandos.

## Proceso seguido

1. **Cuenta en GitHub:** registro en github.com.
2. **Instalación de Git:** descarga desde git-scm.com y verificación con `git --version`.
3. **Configuración de identidad:**

```bash
   git config --global user.name "Andres Felipe Amaya Camacho"
   git config --global user.email "amaya.andres1@uniagraria.edu.co"
   ```

4. **Creación del repositorio** `tutorial-git-actividad2` en GitHub con un README inicial.
5. **Clonación en local:**

```bash
   git clone https://github.com/andresfel423-png/tutorial-git-actividad2.git
   cd tutorial-git-actividad2
   ```

6. **Elaboración de los capítulos** en Word, uno por capítulo de *Pro Git*, y exportación de cada uno a PDF.
7. **Ciclo de trabajo por capítulo:** `git add` → `git commit` → `git push`, al terminar cada capítulo.
8. **Documentación** del proceso en este README.

## Comandos utilizados

|Comando|Para qué se usó|
|-|-|
|`git --version`|Verificar que Git está instalado|
|`git config --global ...`|Definir nombre y correo del autor de los commits|
|`git clone <url>`|Copiar el repositorio de GitHub al equipo local|
|`git status`|Ver qué archivos cambiaron o están preparados|
|`git add <archivos>`|Preparar los cambios para el commit|
|`git commit -m "mensaje"`|Guardar los cambios en el historial con un mensaje descriptivo|
|`git push origin main`|Enviar los commits locales al repositorio en GitHub|
|`git log --oneline`|Revisar el historial de commits|

Ejemplo del ciclo aplicado a un capítulo:

```bash
git add capitulos/Capitulo01\_Inicio.docx capitulos/Capitulo01\_Inicio.pdf
git commit -m "Agrega capítulo 1: Inicio (control de versiones e instalación)"
git push origin main
```

## Contenido del repositorio

```
tutorial-git-actividad2/
├── README.md
├── bitacora.txt
├── logo\_uniagraria.png
└── capitulos/
    ├── Capitulo01\_Inicio (.docx / .pdf)
    ├── Capitulo02\_Fundamentos\_de\_Git
    ├── Capitulo03\_Ramas\_en\_Git
    ├── Capitulo04\_Git\_en\_el\_servidor
    ├── Capitulo05\_Git\_en\_entornos\_distribuidos
    ├── Capitulo06\_GitHub
    ├── Capitulo07\_Herramientas\_de\_Git
    ├── Capitulo08\_Personalizacion\_de\_Git
    ├── Capitulo09\_Git\_y\_otros\_sistemas
    └── Capitulo10\_Funcionamiento\_interno\_de\_Git
```

|Capítulo|Tema|
|-|-|
|1|Inicio: control de versiones, instalación y configuración|
|2|Fundamentos de Git: init, clone, add, commit, log, deshacer, remotos, etiquetas|
|3|Ramas en Git: branch, merge, conflictos, rebase|
|4|Git en el servidor: protocolos, SSH, opciones de alojamiento|
|5|Git en entornos distribuidos: flujos de trabajo, contribuir y mantener proyectos|
|6|GitHub: cuenta, forks, pull requests, organizaciones|
|7|Herramientas de Git: revisiones, stash, reset, bisect, submódulos|
|8|Personalización de Git: configuración, atributos y ganchos|
|9|Git y otros sistemas: git svn y migración|
|10|Funcionamiento interno: objetos, referencias, packfiles|

## Cambios realizados por commit

> Ajuste esta tabla para que coincida con su historial real (`git log --oneline`).

|Commit (mensaje)|Cambio|
|-|-|
|Agrega bitácora inicial|Se crea `bitacora.txt`|
|Agrega capítulo 1: Inicio|Documento Word y PDF del capítulo 1|
|Agrega capítulo 2: Fundamentos de Git|Documento Word y PDF del capítulo 2|
|Agrega capítulo 3: Ramas en Git|Documento Word y PDF del capítulo 3|
|Agrega capítulo 4: Git en el servidor|Documento Word y PDF del capítulo 4|
|Agrega capítulo 5: Git en entornos distribuidos|Documento Word y PDF del capítulo 5|
|Agrega capítulo 6: GitHub|Documento Word y PDF del capítulo 6|
|Agrega capítulo 7: Herramientas de Git|Documento Word y PDF del capítulo 7|
|Agrega capítulo 8: Personalización de Git|Documento Word y PDF del capítulo 8|
|Agrega capítulo 9: Git y otros sistemas|Documento Word y PDF del capítulo 9|
|Agrega capítulo 10: Funcionamiento interno|Documento Word y PDF del capítulo 10|
|Actualiza bitácora con avances|Se registran avances y dificultades en `bitacora.txt`|
|Agrega README con documentación del proceso|Se crea este archivo|

## Dificultades y soluciones

> Reemplace esta sección con las dificultades reales que tuvo.

* **Error de autenticación en `git push`:** GitHub no acepta la contraseña de la cuenta; se resolvió con un Personal Access Token (o una clave SSH).
* **Rama `master` vs `main`:** se unificó con `git branch -M main`.

## Referencias

* Chacon, S., \& Straub, B. (2014). *Pro Git* (2nd ed.). Apress. https://git-scm.com/book/es/v2
* GitHub, Inc. (2019). *GitHub Guides: Learn Git and GitHub* (2nd ed.). https://guides.github.com/
* Hutch Data Science. (s.f.). *Using GitHub in a workflow*. https://hutchdatascience.org/Tools\_for\_Reproducible\_Workflows\_in\_R/using-github-in-a-workflow.html

