# Project Documentation

Comprehensive documentation is mandatory. For any new project, you will create a `README.md` file and a `/docs` folder if one doesn't exist. The creation and level of detail of the following documents should be proportional to the scale and complexity of the project. For small tasks or scripts, updating the `README.md` and providing clear code comments may be sufficient.

These will be populated with the following:

### Root Directory Files

*   `README.md`: A top-level summary of the project, its purpose, and instructions for setup and usage.
*   `LICENSE`: The legal license under which the project is available.

### Documentation Folder (`/docs`)

*   `/docs/product-requirements-document.md`: Capturing user's needs and goals. Outlining project's vision, features, and scope.
*   `/docs/software-requirements-specification.md`: A detailed description of the system's functional and non-functional requirements.
*   `/docs/backlog.md`: The master blueprint and single source of truth for what the project aims to achieve. This is a living document that outlines the entire scope of work, broken down into phases and actionable tasks.
    *   **Structure:** Use checklists (`[ ]`, `[~]`, `[x]`) to track the status of major phases and individual tasks.
*   `/docs/prose_styleguide.md`: Defines the personality and tone of all written content (documentation, UI text, commit messages) to ensure a consistent voice.
*   `/docs/code_styleguide.md`: Enforces coding consistency. It defines the rules for all code to ensure it's readable, maintainable, and consistent.
    *   **Structure:** State a core principle (e.g., "Clarity Over Cleverness"), link to base style guides (like PEP 8), and add project-specific overrides for naming conventions, import order, comment style, etc.
*   `/docs/architecture-design-document.md`: Describing the overall architecture and system design, including the *why* behind the choices.
*   `/docs/technical-design-document.md`: Detailing the implementation plan for specific components.
*   `/docs/testing-strategy.md`: Outlining the testing approach, including unit tests, integration tests, and end-to-end tests. It should also define the quality assurance process.

All documentation is considered "live" and must be kept in sync with the project's current state.

### Keeping Documentation in Sync

This means that any change in the project, from a new user requirement to a small code refactor, should be reflected in the documentation.

**Example: A User Adds a New Requirement**

When a user requests a new feature (e.g., "add a dark mode to the UI"), the following documents should be updated in sequence:

1.  **Requirements & Vision:**
    *   `/docs/product-requirements-document.md`: Update to reflect the new feature in the project's scope and vision.
    *   `/docs/software-requirements-specification.md`: Add the detailed functional (e.g., "the UI must have a toggle to switch between light and dark mode") and non-functional (e.g., "the theme change should be instantaneous") requirements.

2.  **Task Planning:**
    *   `/docs/backlog.md`: Create new tasks for designing, implementing, and testing the dark mode feature. Use checklists to track progress.

3.  **Design:**
    *   `/docs/architecture-design-document.md`: If the change impacts the overall design (e.g., requires a new theme management system), update this document.
    *   `/docs/technical-design-document.md`: Detail the implementation plan, including the CSS variables, theme switching logic, and component-specific changes.

4.  **Testing:**
    *   `/docs/testing-strategy.md`: Add test cases for the new feature, including UI tests for the theme switch and visual regression tests.
