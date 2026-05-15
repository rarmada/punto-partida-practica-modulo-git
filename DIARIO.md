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



```
  id: 5,
  title: "Opción 5",
  description: "Pull Request",
  message:
    "Una Pull Request es una propuesta formal para incorporar cambios de una rama a otra. Permite revisar el código antes de mergear y deja un historial claro de qué se hizo y por qué.",
  featureFlag: false,
},
