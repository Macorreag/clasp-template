# Google Apps Script Starter Template with clasp

[![clasp](https://img.shields.io/badge/built%20with-clasp-4285f4.svg)](https://github.com/google/clasp)

## About

This repository is a starter template for Google Apps Script projects using clasp (Command Line Apps Script Projects). It simplifies the development and deployment of Apps Script projects by providing a structured setup.

Inspired by [howdy39/gas-clasp-starter](https://github.com/howdy39/gas-clasp-starter), this template is ideal for developers looking to streamline their Apps Script workflows.

## Features
- Easy setup for Apps Script projects
- Integration with clasp for command-line management
- Structured directory for better organization
- Autocomplete for Google Apps Script classes in VSCode
- Watch mode for automatic deployment

![Autocomplete for classes of Google Apps Script in VSCode](autocomplete.png)

## Installation

Follow these steps to set up the project:

1. Install clasp globally:
   ```bash
   npm install -g @google/clasp
   ```

2. Log in to clasp:
   ```bash
   clasp login
   ```

3. Initialize a new project:
   ```bash
   npm init
   ```

4. Create a `src` directory and clone your script:
   ```bash
   mkdir src
   ```

5. Install Google Apps Script types for autocomplete:
   ```bash
   npm i -S @types/google-apps-script   
   ```

6. Navigate to the `src` directory and clone your Apps Script project:
   ```bash
   cd src
   clasp clone "SCRIPT-ID" --rootDir .
   ```

> When cloning, the `.claspignore` file won't be tracked, but files defined in this file will be omitted.

7. To verify files in an existing project:
   ```bash
   clasp status
   ```

## How to Use

Once your project is set up, you can use the following clasp commands:

- **Push your local changes to Apps Script:**
  ```bash
  clasp push
  ```

- **Pull changes from Apps Script to your local directory:**
  ```bash
  clasp pull
  ```

- **Push changes automatically on save (watch mode):**
  ```bash
  clasp push -w
  ```

## Resources
- [Official clasp documentation](https://github.com/google/clasp)
- [howdy39/gas-clasp-starter](https://github.com/howdy39/gas-clasp-starter)
- [Learn Google Spreadsheets tutorial](https://www.youtube.com/watch?v=4Qlt3p6N0es&ab_channel=LearnGoogleSpreadsheets)

## License
MIT