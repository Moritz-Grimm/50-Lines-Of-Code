# Contributing Guide

Thank you for your interest in contributing to this project!  
Here’s how to submit your mini project:

## How to contribute

1. Fork the repository
2. Create a new branch following the naming convention => ``language_projectName``
3. Add your new project in the correct language folder
4. Create a pull request after checking all [requirements](#-requirements)

---

## ✅ Requirements

- [ ] Must be **executable** (compiles or runs without errors)
- [ ] **Max 50 lines of code** (excluding comments and empty lines)
- [ ] **No external libraries** (standard library only)
- [ ] Add your project to the appropriate **language folder** => LanguageInitial/Language/ProjectName/ProjectFile + README.md
- [ ] Project folder name should be the name of your project
- [ ] Fill in a `README.md` inside your project folder with the help of the template. For an example on how to it should be look into one of the [Example Projects](#example-projects)
- [ ] Update the [README](README.md) language index with your language and project
- [ ] If you're adding a project in a language that doesn't have any tests yet, please create a new test
- [ ] If you're adding a project requiring user input, please add a test to proof your project compiles and works correctly. For further information on how to do it correctly please refer to [this](#adding-a-universal-language-workflow-or-writing-a-custom-one)
- [ ] Add a .gitignore file for your project if necessary to exclude unwanted files (such as build artifacts, temporary files, or IDE-specific configurations) from being committed with your project

---

## ❗ Important Notes
Please make sure **all** requirements are met for your contribution to be accepted.<br>
If you have any questions or something is unclear, feel free to open a issue!

---

## Adding a universal language workflow or writing a custom one
### Adding a universal language workflow
There is not much to take into account when writing a universal workflow, simply follow this easy language convention ``language.yaml`` <br>
You can also refer to one of these tests
- [Python Workflow](/.github/workflows/python.yaml)
- [Brainfuck Workflow](/.github/workflows/brainfuck.yaml)

### Adding a custom workflow
When writing your own test, please follow this steps
1. Create a .yaml file following this naming conventions => ``language_projectName.yaml``
2. Give it a name based on this => ``language filename 'test'``
3. Always add this restrictions: 
    ``on:
        pull_request: 
            branches: [ "main" ] 
            types: [opened, synchronize, reopened] 
        workflow_dispatch:``

Also, here is a example on how to do it correctly
- [Python simple_number_input.yaml](/.github/workflows/python_simpleNumberInput.yaml)

---

## Example Projects

### Brainfuck
- [Hello World – README](/b/brainfuck/HelloWorld/README.md)

### C#
- [Hello World – README](/c/c-sharp/HelloWorld/README.md)

### Python
- [Hello World – README](/p/python/hello_world/README.md)
- [Simple Number Input - README](/p/python/simple_number_input/README.md)

