# Contributing to Intelli Chorus Recorder

First off, thank you for considering contributing! The **Intelli Chorus Recorder** is an open-source initiative from **Unique Creators**, and we welcome developers, audio engineers, and sound designers to help us refine and expand its capabilities. 

At Unique Creators, we practice **Universal Design**. We do not build "for the blind"; we engineer mainstream products where accessibility is the core architecture, not an afterthought. If you share this vision, you are in the right place.

## How Can I Contribute?

There are many ways to contribute, and not all of them involve writing code:

- **Reporting Bugs:** If you discover a bug, please open an issue on our GitHub repository. Provide detailed steps to reproduce it, your REAPER version, OS details, and the screen reader (if applicable).
- **Suggesting Enhancements:** Have an idea for a new feature or workflow automation? Open an issue and describe your vision.
- **Improving Documentation:** Documentation is just as important as code. If you find gaps in our `README.md` or code comments, PRs are highly appreciated.
- **Submitting Code:** Ready to build? We welcome bug fixes, new features, and modular optimizations.

## Code Contribution Guidelines

To ensure the project remains hyper-maintainable, scalable, and rigidly accessible, please adhere strictly to these paradigms when submitting code:

### 1. Project Structure

The script architecture is thoroughly modularized, separating UI, logic, and structure. Please respect this separation of concerns:

- `main.lua`: The orchestrator. Manages initialization, module loading, and top-level execution flows.
- `config.lua`: The central hub for default settings, validation rules, and all user-facing text strings. **Rule:** Never hard-code a string or parameter in another module.
- `ui_wizard.lua`: Exclusively handles user interaction and persistence logic (`.ini` parsing/writing). All dialogs and prompts live here.
- `core_logic.lua`: Contains the core recording, automation, and REAPER API interactions. *Must remain 100% devoid of UI prompts.*
- `lib/utils.lua`: For generic, decoupled utility functions and error reporting capable of reuse across our ecosystem.

### 2. Coding Philosophy & Style

- **Universality & Usability:** *Mandatory.* There are no separate "blind modes." We build a single, unified interface usable by all. Any new features must seamlessly integrate auditory feedback (`utils.speak`) for non-visual operations. Feedback sounds or conversational speech flows are essential.
- **DRY Architecture:** Modular functions, scalable coding, maintainable logic, and utility-driven architecture. Reuse where possible.
- **Comments & Documentation:** Code should explain itself. Comment minimally, exclusively reserving comments for complex logic blocks or regular expressions.
- **Robust Error Handling:** No silent crashes! Functions executing API calls should gracefully catch errors. Use paired returns (`ok, result_or_error`) for verifiable functions. Provide user-friendly, non-cryptic error messages.

### 3. Submitting a Pull Request

Ready to merge? Follow the standard GitHub collaborative flow:

1. **Fork** the repository.
2. **Create a branch** for your feature or bugfix (`git checkout -b feature/your-amazing-feature`).
3. **Commit** your changes following our guidelines, with clean, descriptive commit messages.
4. **Test** your changes thoroughly over an actual recording session within REAPER.
5. **Push** your branch to your fork (`git push origin feature/your-amazing-feature`).
6. **Open a Pull Request** against the main repository, strictly detailing what you changed, why you changed it, and how it aligns with the Universal Design philosophy.

Thank you for helping us build elite tools for the global audio community!

*We are Unique Creators, and creation is our passion!*