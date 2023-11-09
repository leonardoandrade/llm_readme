# AI Summary README Generator

AI Summary is a utility designed to automate the generation of README files for code projects. By analyzing the contents of a project's directory and incorporating recent Git commit messages, it produces a comprehensive summary intended to clearly convey the project's purpose and instructions for its use.

## Features 🚀

- Directory scanning and file content reading with binary file detection
- Prompt generation from file contents and Git commit messages
- Integration with OpenAI's GPT models for summary creation
- Command-line interface for straightforward interaction
- Changelog generation from recent Git commits

## Installation 📦

Before using AI Summary, ensure you have Python and necessary packages installed. Install the required packages using:

```
pip install -r requirements.txt
```

## Usage 🛠️

Set the `OPEN_AI_KEY` environment variable with your OpenAI API key. Run `main.py` with the following arguments:

- `directory`: Path to the directory containing files for processing
- `target_file`: Path where the generated README.md will be saved
- Optional flags:
  - `--generate-changelog`: Boolean to include a changelog (default: True)
  - `--model`: OpenAI model to use (default: gpt-4-1106-preview)
  - `--num-lines`: Number of lines to read from each file (default: 200)

Example command:

```
python main.py ./my_project ./README.md --generate-changelog --model gpt-4-1106-preview --num-lines 200
```

## Latest Changes 🔄

- Introduced reading of latest commit messages for changelog
- Enabled model specification via command-line
- Improved README formatting
- Fixed issues in test cases

## TODOS 📝

- Implement feature for specifying target README size
- Improve error handling and expand logging capabilities
- Assess and integrate user feedback for feature enhancement

**LLM-generated by [AI summarizer](https://github.com/leonardoandrade/llm_readme)**