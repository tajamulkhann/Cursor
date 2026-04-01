# Principles Behind Good Prompting

## Principle 1: Write Clear and Specific Instructions

- **Tactic 1: Use delimiters**
  - Triple quotes: `"""`
  - Triple backticks: ```
  - Triple dashes: ---
  - Angle brackets: `< >`
  - XML tags: `<tag> </tag>`

- **Tactic 2: Ask for structured output**
  - Examples: HTML, JSON

- **Tactic 3: Check whether conditions are satisfied**
  - Verify assumptions required to do the task

- **Tactic 4: Few-shot prompting**
  - Provide successful examples of completing tasks  
  - Then ask the model to perform the task

---

## Principle 2: Give the Model Time to Think

- **Tactic 1: Specify the steps to complete a task**
  - Step 1: ...
  - Step 2: ...
  - ...
  - Step N: ...

- **Tactic 2: Instruct the model to work out its own solution before rushing to a conclusion**
