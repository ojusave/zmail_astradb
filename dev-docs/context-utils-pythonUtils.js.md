

---
# High Level Context
## context
**Last Updated at:** 9/30/2024, 8:14:22 PM

# pythonUtils.js Documentation

## Overview
This JavaScript module provides utilities for executing Python scripts from Node.js. It includes functions to find the Python executable and run Python scripts with arguments, capturing their output and handling errors.

## Methods

### getPythonCommand()
Finds and returns the available Python command on the system.

### runPythonScript(scriptPath, ...args)
Executes a Python script with the given arguments and returns a Promise with the script's output.

Example usage:
```javascript
const { runPythonScript } = require('./pythonUtils');

runPythonScript('path/to/script.py', 'arg1', 'arg2')
  .then(output => console.log('Script output:', output))
  .catch(error => console.error('Script error:', error));
```
