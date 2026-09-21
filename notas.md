# Guía Básica: Git y GitHub

Esta guía contiene una explicación sencilla y clara sobre los conceptos fundamentales del control de versiones utilizando **Git** y la plataforma **GitHub**.

---

## 1. ¿Qué es Git?
**Git** es un sistema de control de versiones distribuido (*DVCS* por sus siglas en inglés) de código abierto. Fue creado por Linus Torvalds en 2005.

Su función principal es realizar un seguimiento de los cambios en el código fuente o en cualquier conjunto de archivos a lo largo del tiempo. Permite a los desarrolladores:
- Guardar el historial completo de un proyecto.
- Regresar a versiones anteriores en caso de un error.
- Trabajar en equipo de manera simultánea sin sobrescribir el trabajo de los demás.

*Nota:* Git se ejecuta de forma **local** en tu computadora.

---

## 2. ¿Qué es GitHub?
**GitHub** es una plataforma basada en la nube que permite alojar proyectos y repositorios utilizando el sistema de control de versiones **Git**.

Además de alojar el código, GitHub ofrece herramientas avanzadas para la colaboración y gestión de proyectos, tales como:
- Interfaz gráfica web para explorar el código e historial.
- Gestión de tareas e incidencias (*Issues*).
- Revisión de código colaborativa.
- Integración y despliegue continuo (*CI/CD*).

---

## 3. Diferencia entre Git vs GitHub

Aunque están estrechamente relacionados, **no son lo mismo**:

| Característica | Git | GitHub |
| :--- | :--- | :--- |
| **Tipo** | Software / Herramienta CLI | Servicio web / Plataforma en la nube |
| **Ubicación** | Se instala y ejecuta localmente en tu equipo | Vive en servidores en la nube de Microsoft/GitHub |
| **Función principal** | Controlar las versiones del código y sus cambios | Alojar los repositorios de Git y facilitar la colaboración |
| **Dependencia** | No requiere conexión a internet para funcionar | Requiere conexión a internet para acceder a la plataforma |
| **Interfaz** | Línea de comandos (CLI) o clientes GUI locales | Interfaz web intuitiva |

*En resumen:* **Git** es la herramienta (el motor) y **GitHub** es el lugar donde guardas y compartes el trabajo realizado con esa herramienta.

---

## 4. ¿Qué es un Commit?
Un **Commit** es una instantánea (*snapshot*) o foto fija del estado de tu proyecto en un momento determinado. 

Cada vez que realizas un *commit*, guardas un paquete de cambios en el historial de Git. Cada commit incluye:
- Un identificador único (un código alfanumérico llamado hash SHA-1).
- Un **mensaje descriptivo** escrito por el desarrollador que explica qué cambios se hicieron.
- Información del autor y la fecha/hora de la modificación.

---

## 5. ¿Qué es un Branch (Rama)?
Una **Branch** (o rama) es una línea independiente de desarrollo dentro de un proyecto.

Por defecto, los proyectos tienen una rama principal (usualmente llamada `main` o `master`). Crear una nueva rama te permite:
- Desarrollar una nueva funcionalidad (*feature*) o corregir un error (*bugfix*) de forma aislada.
- Experimentar con el código sin alterar la versión estable del proyecto principal.

Una vez que el trabajo en la rama está listo y probado, se puede fusionar (*merge*) de nuevo con la rama principal.

---

## 6. ¿Qué es un Pull Request (PR)?
Un **Pull Request** (o PR) es una funcionalidad propia de plataformas como GitHub (no de Git directamente) que se utiliza para solicitar la integración de los cambios de una rama a otra (por ejemplo, enviar los cambios de una rama secundaria a la rama `main`).

El flujo de un Pull Request permite:
1. **Notificar** al equipo que hay un trabajo listo para ser revisado.
2. **Revisar el código** (*Code Review*): otros desarrolladores pueden comentar, hacer preguntas o sugerir mejoras sobre las líneas de código cambiadas.
3. **Aprobar y Fusionar**: Una vez revisado y aprobado, el PR se acepta y los cambios se fusionan (*merge*) con la rama de destino.