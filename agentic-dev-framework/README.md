# Gemini-CLI Agentic Dev Framework
A project to create a repeteable process to build a framework which instruct Gemini CLI on how to work on a code project, following specific guidelines.

Instead of manually writing and maintain a complex and articulated GEMINI.md defining the new project guidelines, and copy that file in the new project to work on, this project define atomic and simple-to-maintain "guidelines building blocks", and define a way to assemple all of them in a final framework files to copy in the new project. In this way, it is possible to use Gemini help to combine the building block, check for coherency, enrich with specific model's knowledge etc.

Yep, kind of very meta ;)


## Project structure

- `GEMINI.md` contain the prompt to combine the guidelines building block and assemble the final framework in the `output` directory

- `block-01-framework_version.md` contain the version of the framework
- `block-01-gemini_md.md` defines the instuctions to build the final GEMINI.md framework file
- `block-03-documentation.md` defines how to organize the documentation of the project


## How to use this proejct

Build the agentic framework
- Launch gemini-cli `gemini` in the main project folder
- Input this prompt: `build the framework`
- Gemini-CLI will create an `output` folder, with all the framework files

Create a new project using the agentic framework
- Create a new folder containing the new project
- Copy the content of the output directory into this new folder
- Launch gemini-cli `gemini` in the main project folder
- Start building the project interacting with Gemini-CLI


## Inspirations
The following ideas inspired this project
- [ksprashu / GEMINI.md](https://gist.github.com/ksprashu/6ff099d07eea9b768631a230a7527a52)
- [Keith's Conductor project](https://github.com/keithballinger/.conductor) 


