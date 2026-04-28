# Copy For LLM (To Clipboard)

Useful BASH script for developing with open-access LLM tools like Chat Jippity, Claudi-bot, and Geminini

Works for mac only (as it depends on `pbcopy`)
```sh
ln -s /path/to/copy_for_llm/main ~/bin/copy_for_llm
```

Then, in the dir you want to copy:

```
copy_for_llm
```

Will copy everything in your current directory

To exclude a file or folder:

```
echo "node_modules" >> .llmignore
```
