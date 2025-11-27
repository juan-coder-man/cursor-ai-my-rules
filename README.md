# cursor-ai-my-rules

Custom user rules for Cursor AI

## User Rules

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

### 9. Component Architecture and Encapsulation

- Favour small, focused, reusable components/widgets with a single responsibility
- Encapsulate layout, behaviour, and styles inside components; do not leak implementation details
- Extract a new component when a visual or structural pattern is repeated more than once
- Do not mix business logic with UI logic: keep data fetching, state orchestration, and domain rules outside of presentational components
- Prefer composition over inheritance when building UI components
- Use clear, descriptive names that reflect the component's role (e.g. PrimaryButton, FormFieldLabel, CardContainer)
- Avoid "god components" with too many responsibilities, props, or conditional branches

### 10. Atomic Design and Reusability

- Follow atomic design principles: Atoms → Molecules → Organisms → Templates → Pages
- Atoms: smallest visual units (buttons, icons, inputs, labels, spacers)
- Molecules: small compositions of atoms (input + label + error message, card header, list item)
- Organisms: complex sections built from molecules and atoms (forms, navbars, sidebars, cards with actions)
- Templates/Pages: layout-level structures that compose organisms without redefining visual details
- When adding new UI, first verify if it can be composed using existing atoms/molecules/organisms instead of creating new ones
- Centralize reusable tokens for design (spacing, typography, colours, border-radius, shadows) instead of hardcoding values in multiple places

### 11. Visual Design, Minimalism and UX

- Default to a modern and minimal visual style unless explicitly requested otherwise
- Remove or avoid any decorative element that does not add functional or communicative value
- Prefer simple shapes, limited colour palettes, and consistent spacing over gradients, heavy shadows, and visual noise
- Maintain consistent typographic hierarchy (titles, subtitles, body, captions) across the whole UI
- Use consistent spacing scale and alignment rules; avoid arbitrary paddings/margins
- Ensure all interactive elements (buttons, links, inputs) have clear affordances and hover/active/disabled states
- Keep layouts responsive and adaptable to different screen sizes when applicable
- Avoid long, dense blocks of content; use grouping, whitespace, and clear sectioning for better readability
- Preserve or improve accessibility: readable contrasts, sufficient font sizes, clear focus states, and meaningful labels

### 12. How to Add These Rules

To add these rules to Cursor AI:

1. Open **Settings**
2. Navigate to **Rules and Memories**
3. Select **User Rules**
4. Click **Add Rules**
5. Copy and paste the rules from the sections below

## Project Rules

To add project-specific rules for a particular language or framework:

1. Create a rule file in your project root with the language/framework name (e.g., `default-flutter.md`, `default-typescript.md`)
2. Use the `.md` format with frontmatter metadata:
   ```markdown
   ---
   description:
   globs:
   alwaysApply: true
   ---
   ```
3. Add your language or framework-specific rules in the file
4. Convert the `.md` file to `.mdc` format before adding it to the editor
5. In Cursor AI:
   - Open **Settings**
   - Navigate to **Rules and Memories**
   - Select **Project Rules**
   - Click **Add Rules from File**
   - Select your `.mdc` rule file

This allows you to have specific coding standards and patterns for different languages or frameworks within your project.
