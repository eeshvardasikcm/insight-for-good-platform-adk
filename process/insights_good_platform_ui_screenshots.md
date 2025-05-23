# Insights for Good Platform - Initial UI Plan: Minimal MVP with Extensible Text Interaction

### Goal: Achieving MVP and a Runnable Submission by the Deadline with Extensible Text Input

The primary goal is to develop a **minimal manual-entry UI** centered around a text input for the "Insights for Good Platform." This UI will allow judges (and future users) to interact with the core logic of the MVP through text, providing input and receiving output. It will also facilitate the association of **images (screenshots demonstrating MVP features)**, and a sequential review of these interactions. This streamlined UI will be the foundation for the platform's initial MVP and its submission, directly showcasing how key features are demonstrated and how the system can be extended.

---

### Core UI Features (Demonstrating Minimal MVP with Extensibility)

* **Primary Text Input/Output Area:** A central text box or console-like area where users can type commands, queries, or data, and receive text-based responses or system output. This is the primary interaction point.
* **Simple Manual Data and Image Entry (for Submission Documentation):** Alongside the interactive text area, a separate, clear mechanism for **uploading or selecting an image (a screenshot serving as visual evidence of an MVP feature)**. This is specifically for documenting the features demonstrated *via* the text interaction.
* **Contextual Input for MVP Features:** Intuitive UI elements for immediately recording the context and rationale associated with a *specific text interaction* and its linked image. This manual text input will highlight its contribution to the MVP, explaining "the why" behind that demonstrated feature.
* **Sequential Display of MVP Feature Demonstrations:** Text interaction logs and their associated images (screenshots of MVP features) will be manually indexed and linked to the sequence in which they are added. This order will directly represent the demonstration flow of your MVP features for the submission.
* **Emphasis on Extensibility through Text Commands:** The design will implicitly convey how new functionalities can be added by expanding the range of recognized text commands or the complexity of text-based interactions.

---

### UI Planning Stages (Initial Focus for MVP Submission)

#### Phase 1: Design of Interactive Text Box and Output Area (Core MVP Interaction)

Focus on the central text interaction. This will be the primary way judges interact with your MVP's logic.

* **Interactive Text Input Field:**
    * A prominent, single-line text input field (or multi-line, if direct multi-line commands are expected for the MVP).
    * A "Submit" or "Enter" button (or allow pressing Enter key) to send the input.
    * Consider a clear placeholder text (e.g., "Enter command...", "Type your query here...")
* **Output/Response Display Area:**
    * A larger, read-only text area (e.g., a scrollable div or text box) to display the application's responses, results, or current state based on the text input. This mimics a console or chat interface.
* **Initial Commands/Interactions for MVP:** Define 1-2 core text commands/inputs that demonstrate the absolute minimum functionality of your MVP. For example:
    * `list_data`: Displays some predefined data.
    * `add_item [item_name]`: Adds a simple item to an internal list.
    * `query [keyword]`: Simulates a basic search.
* **Extensibility Hook:** The very nature of a text command interface implies extensibility. Document this as a core design principle: new commands can be added to the underlying logic without requiring major UI changes.

#### Phase 2: Design of Manual Documentation Area (for Judge Submission)

This is separate from the live interaction but crucial for the *submission*. It allows you to document the specific text interactions and their visual proof.

* **"Document Interaction" Button/Section:** A clear UI element that, when clicked, captures the *current state of the text input/output area* and prompts the user to add a description and an image.
* **Documentation Entry Fields:**
    * **Demonstration Title:** A concise name for the interaction being documented (e.g., "Feature Demo: Listing Data").
    * **Text Interaction Log:** A read-only copy of the relevant input(s) and output(s) from the main text area.
    * **Feature Description/Rationale:** A multi-line text area to explain what this interaction demonstrates, its significance, and how it fulfills an MVP requirement.
    * **"Upload Screenshot" Button:** A mechanism for uploading a screenshot of the UI at that specific interaction point, visually confirming the text output.
    * **Image Preview Area:** A small thumbnail or preview of the uploaded screenshot.

#### Phase 3: Design of Sequential Review and Export (for Judge Evaluation)

Focus on presenting the documented demonstrations clearly and providing an export method.

* **Sequential Demonstration List:**
    * A sidebar or main area listing each documented interaction (e.g., "Demo 1: Data Listing," "Demo 2: Item Addition"). Each item, when clicked, displays its details.
* **Detailed Demonstration View:**
    * When a demonstration is selected, display:
        * **Demonstration Title**
        * **Captured Text Interaction Log**
        * **Associated Screenshot (prominently displayed)**
        * **Feature Description/Rationale**
* **Export Functionality:**
    * **Recommended Export Format: HTML Report or PDF Report.** This self-contained format will present all documented demonstrations (text logs, descriptions, screenshots) in a clear, sequential report that judges can easily review without running your application. This implicitly *demonstrates* the extensibility by showcasing multiple unique interactions.

---

### Next Steps for MVP Submission (Focusing on Runnable Evaluation)

* **Define Minimum Viable Text Interactions:** Clearly specify the 1-2 core commands/inputs that will be fully functional and demonstrate the MVP's essence.
* **Design the Image Upload/Selection Mechanism:** Decide on the user interaction for image upload (e.g., drag-and-drop, traditional file picker) and temporary storage considerations for the images.
* **Create Mockups or Wireframes:** Visually lay out the interactive text box, the documentation entry UI, and the sequential display interface.
* **Consider Judge-Specific Requirements:** If judges need to *run* your application, determine how this documented UI will integrate. Ensure your export plan directly supports how the judges prefer to receive documentation.
