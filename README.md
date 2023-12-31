# AI Summary README Generator

AI Summary is an automated tool designed to streamline the creation of README files for code projects. It analyzes the contents of a project's directory and integrates recent Git commit messages to craft a comprehensive and informative README that outlines the project's purpose and usage instructions.

## Features 🚀

- Scans directories and reads file contents with a keen eye for binary files.
- Generates prompts from file contents and Git commit histories for an AI-powered summary.
- Utilizes OpenAI's GPT models to create informative summaries.
- Offers a command-line interface for seamless user interaction.
- Produces a changelog based on the latest Git commits to keep users informed of recent changes.

## Installation 📦

To set up AI Summary, ensure Python is installed along with all required dependencies. Install the necessary packages with the following command:

```
pip install -r requirements.txt
```

## Usage 🛠️

Define the `OPEN_AI_KEY` environment variable with your OpenAI API key. Execute `main.py` with the specified arguments:

- `directory`: The path to the directory containing files to be processed.
- `target_file`: The path for saving the generated README.md file.
- Optional flags to fine-tune operation:
  - `--generate-changelog`: Include a changelog (default: True).
  - `--model`: Specify the OpenAI model (default: gpt-4-1106-preview).
  - `--num-lines`: Limit the number of lines read from each file (default: 200).

Example usage:

```
python main.py ./my_project ./README.md --generate-changelog --model gpt-4-1106-preview --num-lines 200
```

## Latest Changes 🔄

- Added functionality for recursive directory generation.
- Introduced optional logging of the last prompt.
- Implemented a line limit for file content reading.
- Integrated reading of the latest commit messages for an up-to-date changelog.

## TODOS 📝

- Add a feature to specify the desired size of the README output.
- Enhance error handling and expand logging for better diagnostics and traceability.
- Incorporate user feedback to refine features and improve the user experience.

**AI-generated by [LLM README](https://github.com/leonardoandrade/llm_readme)**