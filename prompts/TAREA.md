# Tarea: Mi prompt avanzado 
 
## Tarea elegida 
 
Generar casos de prueba para un módulo de **Registro de Usuarios**.

## Version 1: prompt basico 

Crea casos de prueba para un registro de usuarios.
 
## Version 2 

<rol>Actúa como QA Tester Senior.</rol>
<tarea>Crea casos de prueba para el registro de usuarios.</tarea>
 
## Version 3: prompt final 
 

<rol>Actúa como QA Tester Senior especialista en pruebas funcionales.</rol>
<contexto>Formulario de registro con nombre, correo y contraseña.</contexto>
<instrucciones>
1. Piensa paso a paso qué validaciones de seguridad y campos obligatorios faltan (Chain of Thought).
2. Genera 4 casos de prueba esenciales.
</instrucciones>
<ejemplos>
| ID | Escenario | Resultado Esperado |
| TC01 | Registro exitoso | Usuario creado correctamente |
</ejemplos>
<formato>Tabla con columnas: ID, Escenario, Datos de Entrada, Resultado Esperado.</formato>

## Tecnicas usadas en el prompt final

| Técnica | Dónde se usa en el prompt |
|---|---|
| **Role Prompting** | `<rol>`: QA Tester Senior |
| **Prompt Estructurado** | Etiquetas XML (`<rol>`, `<contexto>`, etc.) |
| **Chain of Thought** | `<instrucciones>`: "Piensa paso a paso..." |
| **Few-shot** | `<ejemplos>`: Estructura de la tabla |
 
## Evaluacion del resultado

| Criterio | Cumple (Sí / No) |
|---|---|
| ¿Tiene un rol específico? | Sí |
| ¿Usa ejemplos de formato (Few-shot)? | Sí |
| ¿Obliga a pensar paso a paso (Chain of Thought)? | Sí |
| ¿Entrega los resultados en una tabla clara? | Sí |

## Por que elegi estas tecnicas

Elegí estas técnicas para que la IA sepa su rol, organice bien la información, piense antes de responder y me dé el resultado en una tabla limpia.