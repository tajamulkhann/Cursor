# Principles Behind Good Prompting

## Principle 1: Write Clear and Specific Instructions

- **Tactic 1: Use delimiters**
  - Triple quotes: `"""` → Encloses text clearly, often used to separate instructions or examples.
  - Triple backticks: ``` → Marks code blocks or structured text (like JSON, Python, etc.).
  - Triple dashes: --- → Separates sections or emphasizes boundaries in text.
  - Angle brackets: `< >` → Highlights placeholders or variables (e.g., `<name>`).
  - XML tags: `<tag> </tag>` → Defines structured segments, useful for hierarchical or nested data.

- **Tactic 2: Ask for structured output**
  - Examples: HTML, JSON  
  - Ensures the model responds in a predictable, machine-readable format.

- **Tactic 3: Check whether conditions are satisfied**
  - Verify assumptions required to do the task before proceeding.

- **Tactic 4: Few-shot prompting**
  - Provide successful examples of completing tasks.  
  - Then ask the model to perform the task in the same style.

---

## Principle 2: Give the Model Time to Think

- **Tactic 1: Specify the steps to complete a task**
  - Step 1: ...
  - Step 2: ...
  - ...
  - Step N: ...

- **Tactic 2: Instruct the model to work out its own solution before rushing to a conclusion**
