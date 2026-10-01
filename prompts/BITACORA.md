# Bitacora de tecnicas avanzadas

Laboratorio 07: Tecnicas Avanzadas de Prompting.
Herramienta de IA usada: (escribe aqui cual usaste, ej: ChatGPT / Claude / Gemini)

## Ejercicio 2: Zero-shot, one-shot y few-shot

| Tipo | Aciertos (de 5) | Formato de la respuesta | Todas con el mismo formato (Si/No) |
|---|---|---|---|
| Zero-shot | 5 | Tabla con dos columnas (Comentario / Clasificación) | No |
| One-shot | 5 | "Texto" -> Etiqueta | Si |
| Few-shot | 5 | "Texto" -> Etiqueta | Si |

## Ejercicio 3: Chain of Thought

| Pedido | Respuesta de la IA | Muestra los pasos (Si/No) | Correcta (Si/No) |
|---|---|---|---|
| Directo | 318.60 | No | Si |
| Paso a paso | 318.60 -> con expicacion | Si | Si |

### Justificación:
Es útil porque nos permite verificar que el resultado sea correcto y que la IA haya seguido todas las indicaciones dadas. Además, facilita auditar el procedimiento para saber exactamente dónde corregir si ocurre un error.

## Ejercicio 4: Role prompting

| Version | Vocabulario | Usa ejemplos o codigo | A quien le sirve mas |
|---|---|---|---|
| A. Sin rol | Intermedio | Metáfora de caja y código en Python | Principiantes |
| B. Rol docente | Muy sencillo | Ejemplos de juegos y código en Python | Quienes nunca han programado |
| C. Rol senior | Técnico | Código técnico en Java |  Programadores |

## Ejercicio 5: Descomposicion

- **Paso 1:** Entregó los 5 requisitos principales del sistema (CRUD, control de stock, alertas, proveedores y reportes).
- **Paso 2:** Entregó el diseño de 4 clases principales en Java con sus atributos y tipos de datos 
- **Paso 3:** Entregó el código fuente en Java 
- **Paso 4:** Entregó 3 mejoras 

**Comparación:** El pedido de una sola vez generó un resultado general, una mezcla de bases de datos SQL y Python. En cambio el pedido por pasos produjo un diseño organizado en Java que permitió estructurar mejor cada parte del código.

## Ejercicio 6: Prompt estructurado y autocritica

| Qué revisar | Cumple (Sí / No) |
|---|---|
| ¿Tiene las 4 columnas pedidas? | Sí |
| ¿Incluye el bloqueo después de 3 intentos? | Sí |
| ¿Incluye casos con campos vacíos? | Sí |
| ¿Indica qué casos agregó en la autocrítica? | Sí |
| ¿Hay algún caso repetido o que no tenga sentido? | No |

```text
<rol>Actua como analista de pruebas de software.</rol>
<contexto>Login web con correo y contraseña...</contexto>

Mensaje de autocrítica:
Revisa tu tabla: faltan casos límite como campos vacíos, correo sin @ o contraseña con espacios.