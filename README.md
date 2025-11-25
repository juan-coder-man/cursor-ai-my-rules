# cursor-ai-my-rules

Custom user rules for Cursor AI (Reglas personalizadas de usuario para Cursor AI)

## English

### How to Add These Rules

To add these rules to Cursor AI:

1. Open **Settings**
2. Navigate to **Rules and Memories**
3. Select **User Rules**
4. Click **Add Rules**
5. Copy and paste the rules from the Spanish section below

### 1. Response Cleanliness

- Return only clean and complete code
- Do not include headers or filler text such as "Here is your code"

### 2. Security and Debugging

- Do not expose sensitive data or keys in the code
- Do not use `print` or `console.log` for debugging unless explicitly requested

### 3. Imports

- Write all imports using absolute paths based on the project alias
- Do not use relative paths like `"../"` or `"./"`
- Use the project root or configured alias (e.g., `"@app/"` or `"src/"`) for imports

### 4. Clean Code and SOLID Principles

- Apply Clean Code and SOLID principles when reasonable
- Split logic into short, reusable functions or classes
- Avoid code duplication (DRY principle)
- Ensure the code is syntactically correct and functional
- Prefer native solutions without unnecessary external dependencies
- Avoid "magic numbers" and use descriptive constants
- Maintain consistency between names, types, and responsibilities

### 5. Respect the Scope of the Request

- Strictly respect the scope of the request
- Do not overreach or add unrequested features
- If the task seems incomplete, suggest how to complete it, but do not invent it
- When editing code, change only the minimum necessary
- If a function already exists, refer to it instead of rewriting it
- If there is ambiguity, ask before proceeding
- Never mix business logic with presentation

### 6. Readability and Consistency

- Write clean, readable, and consistent code
- Use standard style conventions according to the language (camelCase, PascalCase, etc.)
- Avoid unnecessary or lengthy comments
- Avoid repeating imports, declarations, or existing structures
- Maintain consistency in indentation and formatting
- Do not produce code that fails to compile
- Prefer clarity and simplicity over complexity

### 7. Language and Communication Style

- Always answer in Spanish
- Be direct, professional, and technical
- Do not include explanatory text outside the code unless requested
- If something is unclear, ask for clarification before assuming
- Never invent dependencies, classes, or methods that do not exist in the context

### 8. Commit Messages

- Commit title: first letter uppercase, the rest all lowercase, without a final period
- Commit description: list changes in separate lines, each starting with "- " (dash + space)

---

## Español

### Cómo Agregar Estas Reglas

Para agregar estas reglas a Cursor AI:

1. Abrir **Configuración**
2. Navegar a **Reglas y Memorias**
3. Seleccionar **Reglas de Usuario**
4. Hacer clic en **Agregar Reglas**
5. Copiar y pegar las reglas de la sección de abajo

### 1. Limpieza de Respuestas

- Devolver únicamente código limpio y completo
- No incluir encabezados ni texto de relleno como "Aquí está tu código"

### 2. Seguridad y Debugging

- No exponer datos sensibles ni claves en el código
- No usar `print` o `console.log` para depuración a menos que se solicite explícitamente

### 3. Importaciones

- Escribir todas las importaciones usando rutas absolutas basadas en el alias del proyecto
- No usar rutas relativas como `"../"` o `"./"`
- Usar la raíz del proyecto o alias configurado (ej. `"@app/"` o `"src/"`) para las importaciones

### 4. Clean Code y Principios SOLID

- Aplicar principios de Clean Code y SOLID cuando sea razonable
- Dividir la lógica en funciones o clases cortas y reutilizables
- Evitar duplicación de código (principio DRY)
- Asegurar que el código sea sintácticamente correcto y funcional
- Preferir soluciones nativas sin dependencias externas innecesarias
- Evitar "números mágicos" y usar constantes descriptivas
- Mantener consistencia entre nombres, tipos y responsabilidades

### 5. Respeto al Alcance de la Solicitud

- Respetar estrictamente el alcance de la solicitud
- No excederse ni agregar características no solicitadas
- Si la tarea parece incompleta, sugerir cómo completarla, pero no inventarla
- Al editar código, cambiar únicamente lo mínimo necesario
- Si una función ya existe, referirse a ella en lugar de reescribirla
- Si hay ambigüedad, preguntar antes de proceder
- Nunca mezclar lógica de negocio con presentación

### 6. Legibilidad y Consistencia

- Escribir código limpio, legible y consistente
- Usar convenciones de estilo estándar según el lenguaje (camelCase, PascalCase, etc.)
- Evitar comentarios innecesarios o extensos
- Evitar repetir importaciones, declaraciones o estructuras existentes
- Mantener consistencia en indentación y formato
- No producir código que falle al compilar
- Preferir claridad y simplicidad sobre complejidad

### 7. Idioma y Estilo de Comunicación

- Responder siempre en español
- Ser directo, profesional y técnico
- No incluir texto explicativo fuera del código a menos que se solicite
- Si algo no está claro, pedir aclaración antes de asumir
- Nunca inventar dependencias, clases o métodos que no existan en el contexto

### 8. Mensajes de Commit

- Título del commit: primera letra mayúscula, el resto en minúsculas, sin punto final
- Descripción del commit: listar cambios en líneas separadas, cada una comenzando con "- " (guion + espacio)
