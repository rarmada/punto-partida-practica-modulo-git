Tarea 1 — Fork y configuración inicial
Escribe qué es un fork y para qué sirve upstream. Adjunta la captura 1 y la captura 2.
Ddesde Terminal de vscode he puesto
git remote -v
Captura 1	Terminal con git remote -v mostrando origin y upstream

<img width="2426" height="513" alt="image" src="https://github.com/user-attachments/assets/46ca29ab-f4d0-43a2-a9a8-8e0171a60391" />
Captura 2	GitHub con la rama dev visible en el desplegable de ramas
<img width="3803" height="1762" alt="image" src="https://github.com/user-attachments/assets/2cc4a3aa-3db6-4d8a-ad4d-c3bbbac26534" />

Un fork es una copia completa de un repositorio ajeno en tu propia cuenta de GitHub.
Cuando se hace un fork, el repositorio local tiene por defecto un solo remoto llamado origin, que apunta al fork en GitHub.
El problema es que el repositorio original puede seguir recibiendo cambios. Para poder sincronizarte con él, se añade un segundo remoto llamado convencionalmente upstream.

Tarea 2 — Feature branch A: añadir la Opción 5

 Explica por qué la rama parte de dev y no de main
 La rama parte de dev ya que en un flujo de trabajo profesional con Git, main representa el código estable y en producción, mientras que la rama dev se utiliza para hacer las modificaciones antes de llegar a producción

Captura 3	La app en el navegador con la Opción 5 recién añadida
<img width="1850" height="1340" alt="image" src="https://github.com/user-attachments/assets/9ba2d891-7ae2-4bae-aa17-4e36136732c8" />



Un conflicto en Git ocurre cuando dos ramas han modificado la misma línea del mismo fichero de forma diferente,
