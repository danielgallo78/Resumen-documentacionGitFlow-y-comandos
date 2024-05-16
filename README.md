# Resumen-documentacionGitFlow-y-comandos
Realizo un breve resumen de la documentacion de GitFlow.


GitFlow es una metodología que organiza cómo trabajamos con el código en proyectos de software usando Git. GitFlow nos ayuda a mantener todo organizado y evitar que las cosas se mezclen o se pierdan. Aquí hay una explicación paso a paso de cómo funciona GitFlow:

## 1. Ramas Principales
   - Master: Piensa en esta rama como el libro terminado y publicado. Siempre debe estar en un estado listo para lanzarse.
   - Develop: Esta es como una versión preliminar del libro donde se combinan todas las nuevas ideas y cambios antes de publicarlos.

## 2. Ramas de Soporte
Estas ramas son temporales y se usan para diferentes tareas específicas:

   - Feature Branches (Ramas de Funcionalidad):
     - Propósito: Añadir nuevas características o cambios
     - Origen: Se crean a partir de , develop.
     - Finalización: Cuando la característica está lista, se fusiona de nuevo en develop.

   - Release Branches (Ramas de Lanzamiento):
     - Propósito: Preparar una nueva versión del libro para ser publicada.
     - Origen: Se crean a partir de develop.
     - Finalización: Cuando está lista, se fusiona en master y develop

   - Hotfix Branches -Ramas de Corrección Rápida-
     - Propósito: Arreglar errores en la versión publicada del libro.
     - Origen: Se crean a partir de master.
     - Finalización: Cuando el arreglo está listo, se fusiona de nuevo en master y develop.

## ¿Cómo Funciona GitFlow?

1. Empezando un Proyecto:
   - El proyecto comienza con las ramas master y develop.

2. Añadiendo Nuevas Funcionalidades:
   - Se crea una rama feature para trabajar en una nueva característica.
   - Una vez completada, se fusiona de nuevo en develop.

3. Preparando una Versión para Publicar:
   - Cuando "develop" está listo para una nueva versión, se crea una rama release.
   - Se hacen los últimos ajustes y correcciones.
   - Una vez listo, se fusiona en "master" (que es la versión publicada) y en develop (para que los cambios estén disponibles para futuras características).

4. Arreglando Errores en la Versión Publicada:
   - Si se encuentra un error en master, se crea una rama hotfix
   - Se arregla el error.
   - La solución se fusiona en master y develop.

## Ventajas de GitFlow

Organización: Mantiene todo estructurado y claro.
Paralelismo: Permite a varias personas trabajar en diferentes partes del proyecto sin interferir.
Calidad: Facilita el manejo de errores y la preparación de versiones estables.


