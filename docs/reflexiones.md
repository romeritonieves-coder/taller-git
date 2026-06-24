# Reflexión Técnica - Taller de Git y GitHub

## Preguntas de Reflexión

### 1. ¿Qué problema resuelve publicar cambios en un repositorio remoto?

Publicar cambios en un repositorio remoto resuelve el problema de la colaboración y el respaldo. Permite que todo el equipo tenga acceso a la última versión del proyecto, evita la pérdida de trabajo y facilita el trabajo en equipo distribuido.

### 2. ¿Por qué es necesario traer cambios remotos antes de continuar trabajando?

Es necesario porque si no actualizamos nuestro repositorio local, podemos trabajar sobre una versión desactualizada del proyecto. Esto genera conflictos cuando intentamos integrar nuestros cambios y podemos perder trabajo realizado por otros miembros del equipo.

### 3. ¿Qué ventaja tiene reorganizar una rama antes de integrarla?

Reorganizar una rama con rebase permite mantener un historial lineal y limpio. Facilita la revisión de cambios, reduce conflictos futuros y hace más fácil entender la evolución del proyecto.

### 4. ¿Por qué se producen los conflictos?

Los conflictos se producen cuando dos o más personas modifican la misma parte de un archivo simultáneamente. Git no puede decidir automáticamente qué versión conservar, por lo que requiere intervención manual para resolver la situación.

### 5. ¿Cuál es el proceso lógico para resolver un conflicto correctamente?

1. Identificar los archivos con conflictos
2. Leer ambos lados del conflicto
3. Decidir qué cambios conservar
4. Editar el archivo eliminando los marcadores de conflicto
5. Guardar los cambios
6. Marcar el archivo como resuelto con `git add`
7. Completar la operación con `git commit`

### 6. ¿Por qué conviene limpiar commits antes de hacer un Pull Request?

Limpiar commits hace que el historial sea más claro y fácil de revisar. Permite al revisor entender rápidamente qué cambios se realizaron, facilita la identificación de problemas y demuestra profesionalismo en el desarrollo.

### 7. ¿Qué ventaja tiene aplicar solo un cambio específico desde otra rama?

Permite incorporar únicamente lo que se necesita sin traer cambios experimentales o no probados. Da control fino sobre qué se integra al proyecto y reduce el riesgo de引入r bugs o cambios no deseados.

### 8. ¿Qué riesgos existen al sobrescribir una rama remota?

Los riesgos incluyen pérdida de trabajo de otros desarrolladores, romper el historial del proyecto, eliminar commits importantes y causar conflictos con el equipo. Siempre se debe comunicar antes de realizar operaciones destructivas.

### 9. ¿Qué buenas prácticas aplicaría en un proyecto real?

- Trabajar siempre en ramas independientes
- Escribir mensajes de commit claros y descriptivos
- Hacer pull frecuentemente para mantenerse actualizado
- Revisar el código antes de integrar cambios
- Resolver conflictos lo antes posible
- Limpiar el historial antes de crear Pull Requests

### 10. ¿Qué errores cometió durante el taller y cómo los solucionó?

Durante el taller se cometieron errores como:
- Trabajar directamente en la rama principal: se solucionó creando ramas separadas
- No actualizar el repositorio local: se resolvió haciendo pull antes de continuar
- Mensajes de commit poco descriptivos: se mejoró escribiendo mensajes claros
- No limpiar el historial: se utilizó squash para consolidar commits
