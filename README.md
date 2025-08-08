# prompt-library
Welcome to the **AI Prompt Library** — a curated collection of reusable, role-specific prompt templates for our team to use with **GitHub Copilot**, **ChatGPT**, or other LLM tools.

This library helps us:
- Save time by reusing well-tested prompts.
- Maintain consistent coding, testing, and documentation quality.
- Scale AI usage across different roles and domains.

## 🚀 How to Use a Prompt

1. Navigate to the relevant folder (e.g., `frontend/` for React UI prompts).
2. Open the `.md` file for your use case.
3. Copy the prompt into **GitHub Copilot Chat** or your LLM tool.
4. Replace placeholders like `[Paste code here]` or `[Insert requirement here]` with your actual context.
5. Run the prompt and review the output before committing any generated code.

---

## 🧩 Example

If you need a JPA Entity from a PostgreSQL table:
- Go to `backend/java-entity-generation.md`
- Copy the prompt into **Copilot Agent Mode** with your `.sql` schema open in VS Code.
- Replace `[Paste table schema here]` with your actual table.
- Let the AI generate the code, then validate it.

---

## 📌 Best Practices

- **One task = one prompt** → Prompts should be focused and clear.
- **Provide context** → Always paste relevant code, requirements, or mockups.
- **Be explicit** → Define the format you want (e.g., JSON, Markdown, Java class).
- **Validate output** → AI-generated code is not automatically production-ready.
- **Iterate** → If the output isn’t right, refine the prompt with more details.

---

## 🛠 Adding a New Prompt

1. Pick the right folder (or create one if needed).
2. Create a new `.md` file named after the task (e.g., `react-table-component.md`).
3. Use this template:
   ---
    title: Generate JPA Entity from PostgreSQL Table
    role: backend
    tags: [java, spring-boot, jpa, postgresql]
    version: 1.0
    last_updated: 2025-08-08
    author: rahul.lalwani
    ---
    
    # 🧬 Generate JPA Entity from PostgreSQL Table
    
    ## 🧩 Use-case
    Java developer needs to convert a PostgreSQL table into a Spring Boot JPA entity.
    
    ## 🧠 Prompt
    <Actual Prompt>

How This Helps in Searching
Search by tag:

bash
Copy
Edit
grep -ril "tags:.*react" prompt-library/
→ Lists all prompts tagged for React.

Search by role:

bash
Copy
Edit
grep -ril "role: ba" prompt-library/
→ Lists all prompts for Business Analysts.

Search by keyword in content:

bash
Copy
Edit
grep -ril "JUnit" prompt-library/

📌 Best Practices for Tagging
Keep tags lowercase and use hyphens if needed (spring-boot, next-js).

Always include role (backend, frontend, ba, test, devops, etc.).

Include tech stack in tags (java, react, gcp, postgresql).

Version control — bump version when you modify the prompt meaningfully.

Add last_updated to track freshness.

Use consistent tag vocabulary — define a TAGS.md file listing all allowed tags.
