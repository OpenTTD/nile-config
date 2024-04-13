# Configuration for nile

This repository contains all the configuration for `nile`.

## File / folder structure

- `languages`: contains all the languages known to `nile`, including its properties.
- `projects`: contains all the projects known to `nile`, including its settings.
- `projects.json`: a list of all projects enabled.

## F.A.Q.

### I want to add a new language

Just add the JSON file to the `languages` folder, and add it to any `projects` that is allowed to use this language.

### I want to add a new project

Just add the JSON file to the `projects` folder, and when you want to enable it, list it in `projects.json` too.

### I want to modify properties of a language

Modify the JSON file in the `languages` folder.
Please make sure to write valid (strict) JSON.

### I want to modify settings of a project

Modify the JSON file in the `projects` folder.
Please make sure to write valid (strict) JSON.

### I made changes to the language / project, but they are not visible

Once you merged your changes, GitHub Workflows will redeploy `nile` with the new settings.
This can take a few minutes.

If the changes aren't visible even after a few minutes, check the GitHub Actions logs to see what went wrong.
