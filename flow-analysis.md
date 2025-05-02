Analyze the entire repository and generate a single `md file` with relevant naming into `/notes` directory with the following structure and requirements:

1. **Entry Point**

   - Automatically detect the main entry point(s) for the requested flow/use case.
   - Show the file path(s) and function/class names that kick off the process.

2. **Strategy Design Overview**

   - Explain the strategic role of this use case within the product and codebase.
   - Describe its impact on the overall solution space (see `/notes/overall.md` for context).

3. **High-Level Flow Overview**

   - Describe what this use case does at a bird’s-eye level.
   - Highlight the core technical concepts involved (e.g. async processing, event handling, data modeling, external APIs).
   - Summarize key decision points and branching logic, and why each decision exists.

4. **Special Notes & Comments**

   - Extract any noteworthy code comments but note that `TODO`/`FIXME` annotations are my comment where I add them to help me understand the code base so it might have mistake.
   - Explain how they relate to the flow or indicate design decisions or caveats.

5. **Entities**

   - Identify domain entities (inferred from comments, variable/function/class names).
   - For each entity, list:
     - The files or modules where it appears
     - Its purpose/role in the system
     - Any important fields or methods

6. **Call Flow Diagram**

   - Render a Mermaid sequence diagram showing the end-to-end call flow:
     - Actors (components or modules) on top
     - Method/function calls and major events
     - Annotate with file names or class names for each step
   - Embed as:
     ```mermaid
     sequenceDiagram
       %% your generated steps here
     ```

7. **Navigation & Diving In**
   - For each major section above, include hyperlinks (relative paths) to the source files.
   - Provide “Next Steps” bullets pointing to the specific files or classes for deeper exploration.

**Output**: Write the complete md file in Markdown, saving it to `/notes/README.md`. Do not print anything else to console.

## Log Learning Log

You should keep track on the learning log like a changelog in the `notes/learning_log.md`, with the date grouped all the learnins, and the bulletpoints about what we have learn in summary below the corresponding date. Latest date should be at the top of the markdown. This learning log can allow me to recall where were I left on.

## Log Glossary

Once this is done, visit the `/notes/glossary.md` to put in the new concept, codebase entities we have learned with short summary, purpose and role if applicable. If same thing already exist, simplify update it after consideration.

---

Here is the use case I am after:

{Your use case}

Begin now.
