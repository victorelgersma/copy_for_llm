# Copy For LLM (To Clipboard) 🏄‍♂️

A lightweight BASH utility to bundle your project's source code into a single, LLM-friendly format. Perfect for when you're collaborating with Chat Jippity, Claudi-bot, or Geminini.

## Features
- **Recursive Copying:** Grabs your entire project structure.
- **Smart Formatting:** Prepends each file with an `=== filename ===` header for clear context.
- **Ignore Logic:** Supports a `.llmignore` file (works just like `.gitignore`).
- **Visual Feedback:** Prints a list of copied files to your terminal without polluting your clipboard.

## Installation (macOS)

1. Ensure you have a `~/bin` directory (or somewhere else in your `$PATH`).
2. Symlink the script:

```sh
ln -s /path/to/copy_for_llm/main ~/bin/copy_for_llm
```

## Usage 

Simply run the command in your project root: 

```sh
copy_for_llm
```

## Excluding Files

Create a `.llmignore` file in your project root. The script will skip any files or directories listed (one per line).

```sh
# Example: Ignore bulky or irrelevant folders
echo "node_modules" >> .llmignore
echo "dist" >> .llmignore
echo "temp_notes.txt" >> .llmignore
```

## Requirements

macOS: Depends on pbcopy.
BASH: Built for a standard Unix shell environment.