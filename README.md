# LABORATORIO #1: Control de Versiones Distribuido (CVDS)

Este laboratorio está diseñado para introducirnos en el uso de Git y GitHub, dos herramientas esenciales para el manejo de versiones y la colaboración en proyectos de software. A lo largo de este laboratorio, se aprendieron los conceptos básicos de Git y cómo interactuar con repositorios de GitHub de forma local y remota.

## Objetivos Laboratorio

En este laboratorio aprenderemos a manejar los comandos básicos de GitHub, lo que nos permitirá gestionar versiones y colaborar de manera eficiente. La primera parte del laboratorio se realizará de manera individual, mientras que en la segunda parte se trabajará en pareja, creamos un informe en el cual está todo el proceso.

## INTEGRANTES

**👥 Estudiantes:**

- Juan José Mejía Celis
- Laura Valentina Gutiérrez Rico


## PREGUNTAS:

  Parte I:
    - "¿Para qué sirven y cómo se usan los comandos `git add` y `git commit -m ‘mensaje’ `?"

        - **`git add`**: Este es un comando que se usa para agregar los cambios en los archivos del proyecto al área de preparación.
          Esto es necesario antes de confirmar esos cambios con un `git commit`, seguido de un push.

          ```
          git add <archivo>  # Agrega un archivo específico
          git add .          # Agrega todos los archivos que han sido modificados

          ```

        - **`git commit -m "mensaje"`**: Por otro lado este es un comando se utiliza para confirmar los cambios previamente preparados con `git add`. 
          El `-m` seguido de un mensaje que describa el cambio realizado. Un ejemplo de uso:
          ```
          git commit -m "Actualizando la información en el README"

          ```

**Fuente**
- [Git Docs - Git Commit](https://git-scm.com/docs/git-commit)

   Parte II:
    - "¿Qué sucedió cuando el Owner y el Colaborador intentaron editar el archivo `README.md` al mismo tiempo y subir los cambios?"
 
 	Cuando intentamos editar el mismo archivo al mismo tiempo, siendo Owner y colaborador y hacer un `git push`, **Git detectó un conflicto en la persona que se demoró más en hacer el push**. Esto ocurre porque no sabe qué versión del archivo debe conservar. En este caso, el sistema me mostrará un mensaje de error y no permitirá que suba los cambios hasta que resuelva el conflicto. El procedimiento para resolver esto consiste en estos pasos:

	```
	1. Realizar un `git pull` para traer los cambios del repositorio remoto.
	2. Resolver los conflictos manualmente.
	3. Finalmente, hacer un nuevo `commit` y `push` para actualizar el repositorio.

	"En la parte de Pull Requests, resolvemos el conflicto con las ramas dentro del Git "
	```

        Fuente:
          - [Git Docs - Resolución de Conflictos](https://git-scm.com/book/en/v2/Git-Tools-Advanced-Merging)

   Parte III  
	**1. ¿Hay una mejor forma de trabajar con Git para no tener conflictos?**  

	Buscando en la web y a nivel personal encontramos las siguientes recomendaciones para trabajar con GitHub de manera correcta evitanto conflictos:

	- **Trabajar en ramas separadas**: Cada vez que se van a hacer cambios, se crea una rama nueva (`git branch rama`). Esto nos permite trabajar sin afectar la rama principal y evita problemas con los cambios de los demás

	- **Sincronización frecuente**: Antes de comenzar a trabajar, hacer un `git pull` para traer los últimos cambios del repositorio.

	- **Commits más pequeños pero descriptivos**: En lugar de hacer un commit gigante al final del día, es mejor hacer commits pequeños y frecuentes, esto no solo facilita la revisión del código, sino que también reduce la posibilidad de conflictos grandes y que sean dificiles de solucionar.

**Fuente**: [Git Best Practices](https://www.atlassian.com/git/tutorials/comparing-workflows)  

	**2. ¿Qué es y cómo funciona el Pull Request?**  
	El **Pull Request (PR)** es una dde las herramientas favoritas para los usuarios en GitHub. Básicamente, es una solicitud para que los cambios que hice en mi rama sean revisados e integrados a la rama principal del proyecto (`main` o `master`). Este proceso no solo ayuda a mantener un historial de cambios ordenado, sino que también fomenta la colaboración y el aprendizaje en equipo.  

**Fuente**: [GitHub Pull Requests](https://docs.github.com/en/pull-requests)  


"❤️😊"

