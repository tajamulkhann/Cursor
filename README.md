# Cursor Overview

## Options
- Base chatbots (Copilot / ChatGPT)
- GitHub Copilot
- Cursor / Aider / Codeium / Cline

## Key Factors
- IDE integration
- Context awareness
- Prompt optimization
- Tool usage
- Collaboration
- Customization
- Performance

## Why Cursor?
- VS Code fork with improved UI
- Strong recognition & funding
- Best in our evaluation
- Enterprise plan: $40/user
  - Privacy mode
  - Limited premium requests
- Active community & updates
- Better debugging & navigation
- Strong multi-file awareness

## Extra Considerations
- Security & compliance
- Team scalability
- Multi-language support
- Roadmap alignment
- CI/CD integration

# Cursor Tips & Best Practices

## 🔑 Key Shortcuts and Features

- **Tab Tab → Code Completion**
  - Double-tap `Tab` to trigger AI-powered code completion.
  - Useful for quickly filling in boilerplate or continuing logic.

- **Ctrl + K → Chat About Code**
  - Opens a chat window with the AI agent.
  - Lets you ask questions about the codebase or request improvements.

- **Select Code + Ctrl + K → Contextual Chat**
  - Highlight a specific code block, then press `Ctrl + K`.
  - The agent focuses only on the selected snippet for explanations or fixes.

- **@ → Folder/Context Reference**
  - Use `@` to give the agent context about a folder, file, or project section.
  - Helps the AI understand dependencies and structure.

- **Modes**
  - **Ask Mode:** Query the agent for explanations, debugging help, or suggestions.
  - **Manual Mode:** Apply changes yourself but still leverage AI hints.
  - **Auto Mode (if available):** AI directly edits code with minimal input.

---

## 🧑‍💻 User Rule
- Always produce **clean code**.
- Avoid **over-commenting** (keep comments meaningful).
- Maintain **consistent modularity** (functions, classes, reusable components).

---

## 📂 Project Rules
- Follow language-specific style guides (PEP8 for Python, etc.).
- Ensure unit tests are updated with every major change.
- Keep dependencies minimal and well-documented.
- Enforce privacy/security best practices in enterprise projects.

---

## 🐍 Python Example (Clean Code)

```python
def is_palindrome(word: str) -> bool:
    """
    Check if a given word is a palindrome.
    
    Args:
        word (str): Input string to check.
    
    Returns:
        bool: True if palindrome, False otherwise.
    """
    cleaned = word.lower().replace(" ", "")
    return cleaned == cleaned[::-1]


# Example usage
print(is_palindrome("Racecar"))  # True
print(is_palindrome("Hello"))    # False
```

- Clean code: concise, modular, and readable.
- Minimal comments: only where necessary (docstring explains purpose).
- Consistency: reusable function with clear naming.

Note: Generate Summaries of Repos using www.repomix.com

# Recoomendation

## 📂 Why Add a `.cursor` Folder?

It’s recommended to add a `.cursor` folder at the **root of your repository** because it provides AI context: project description, coding rules, and task lists. This ensures Cursor generates code aligned with your standards and goals.

---

## 📂 Where to Add `.cursor`

Place the `.cursor` folder at the **root of your repo** (same level as `src/`, `README.md`, etc.).

### Inside `.cursor`, include:
- **description.md** → overview of the project, tech stack, coding rules.
- **todo.md** → list of tasks you want Cursor to work on.
- **mcp.json / configs** → metadata, preferences, or additional rules.

👉 Cursor automatically uses `.cursor` as part of the project context.

---

## 🛠 How It Works in Practice

1. **Import Repo** → Open your project in Cursor.  
2. **Add `.cursor` Folder** → Create it at the root.  
3. **Fill Context Files**:
   - `description.md`: “This repo uses Python, follow clean code, modularity, avoid over-commenting.”
   - `todo.md`: “Implement palindrome check, add unit tests, refactor utils.”
4. **Reference in Prompts** → While chatting with Cursor:
   - “See `todo.md` for pending tasks.”
   - “Follow coding rules in `.cursor/description.md`.”
5. **Review Output** → Cursor generates code aligned with your rules and tasks.


