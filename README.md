# hookhook
Git hooks for multi project repository

## Description
If you have multiple project in your repository, it can be tricky to setup git hooks.

HookHook can help you to find and execute specific tasks on every project in your git repository. It is language/platform agnostic.

It works with a file called `.hookhook.yml`. Here is an example
```yaml
- javascript
  condition: find . -name "package.json"
  command: npm run
- python
  condition: find . -name "*requirements.txt"
  command: make
```

It will find every folder identified by condition and try to execute corresponding command

## Contributing

Use [commitizen](https://github.com/commitizen/cz-cli) to help you to format commit messages.