### Notes

Careful when exporting modujles with the ../ and ./

./ references the current working directory
../ references the parent directory.

In the case of exporting modules, whether or not to use ./ and ../ is indicative of the where the file is in the working directory.

Example: I want to export files into my test.js file in the test directory of my project. The files I want to export, are in the parent directory of the test folder.

Export statements in my test file should have ../ to indicate that the files are in the parent folder.

Example: I want to export a function into another file of the same level in the project structure. Then we must use ./ as the files are in the same two levels.

One line command for creating a .gitignore file ignoring just node_modules
touch .gitignore && echo "node_modules/" >> .gitignore && git rm -r --cached node_modules ; git status

Square brackets in the context of documentation as inputs to function means that the parameters are optional to the function.

console.log will add a new line character (\n) to the end of the string. However, in Node we can use process.stdout.write instead to have more control and avoid automatically adding an extra "newline character" at the end each time.
