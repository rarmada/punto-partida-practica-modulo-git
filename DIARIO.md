## Tarea 1 — Fork y configuración inicial
1. Haz un fork del repositorio del instructor en tu cuenta de GitHub.
2. Clona tu fork en tu ordenador.

```
   git clone https://github.com/rarmada/punto-partida-practica-modulo-git.git
```
3.- Entra en la carpeta proyecto-demo, instala las dependencias y arranca la app para confirmar que funciona.
4.- Añade el repositorio del instructor como remote con el nombre upstream.
```
   git clone https://github.com/rarmada/punto-partida-practica-modulo-git.git
```

5. Verifica con git remote -v que tienes tanto origin (tu fork) como upstream (el instructor).
   
   <img width="2297" height="283" alt="image" src="https://github.com/user-attachments/assets/fd405613-907e-4fcc-8daf-707ac1519c84" />

7. Crea la rama dev y súbela a tu fork.
```
git switch -c dev
git push -u origin dev
```
Diario: Escribe qué es un fork y para qué sirve upstream. Adjunta la captura 1 y la captura 2.

## Tarea 2 — Feature branch A: añadir la Opción 5
Crea la rama feature/opcion-5 desde dev.
```
git switch -c feature/opcion-5
```
Abre src/app.tsx y añade la siguiente tarjeta al array OPTIONS
```
  id: 5,
  title: "Opción 5",
  description: "Pull Request",
  message:
    "Una Pull Request es una propuesta formal para incorporar cambios de una rama a otra. Permite revisar el código antes de mergear y deja un historial claro de qué se hizo y por qué.",
  featureFlag: false,
},
```
Además, cambia el campo description de la Opción 3 de su valor actual a:
description: "Flujo de trabajo",
Arranca la app y verifica en el navegador que aparece la Opción 5.
<img width="2027" height="1415" alt="image" src="https://github.com/user-attachments/assets/246fce3f-c5ce-47e4-b512-8bd0bbb0fc49" />
Haz un commit con el mensaje: feat: añadir Opción 5 y actualizar descripción de Opción 3
```
git add .
git commit -m "feat: añadir Opción 5 y actualizar descripción de Opción 3"
```
Sube la rama a tu fork.
```
git push origin feature/opcion-5
```
Diario: Explica por qué la rama parte de dev y no de main.

Siempre trabajamos en la rama Dev que es la de desarrollo

## Tarea 3 — Feature branch B: añadir la Opción 6 (aquí está el conflicto)

Vuelve a dev y crea la rama feature/opcion-6 desde ahí.
```
git switch dev
git switch -c feature/opcion-6
```
Realizamos las modificaciones solicitadas

Haz un commit con el mensaje: feat: añadir Opción 6 y actualizar descripción de Opción 3
```
git add .
git commit -m "feat: añadir Opción 6 y actualizar descripción de Opción 3"
```
Sube la rama a tu fork.
```
git push origin feature/opcion-6
```
Explica qué es un conflicto en Git y por qué se va a producir aquí.
Un conflicto ocurre cuando Git no puede fusionar automáticamente dos ramas porque ambas han modificado las mismas líneas del mismo archivo de forma diferente y no sabe cuál versión conservar.
Hemos modificado la descripción en las dos ramas.

## Tarea 4 — Pull Request 1: Feature A a dev
Abre una Pull Request en GitHub desde feature/opcion-5 hacia dev.
Ponle como título: feat: añadir Opción 5 y actualizar descripción de Opción 3
Antes de mergear, abre la pestaña Files changed y revisa el diff.
Mergea el PR.
Actualiza tu rama dev local con git pull origin dev.
Diario: Explica qué revisaste en la pestaña Files changed y por qué es útil hacerlo antes de mergear. Adjunta la captura 4.

<img width="3779" height="1753" alt="image" src="https://github.com/user-attachments/assets/b7e6a560-fe21-4a7f-ac5a-00bd263c23cd" />


<img width="2466" height="776" alt="image" src="https://github.com/user-attachments/assets/88937feb-9a25-4327-83cf-fd6ac94e6d97" />






