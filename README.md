# SASS Course
## This course provided by [Elzero School](https://elzero.org/study/sass-2021-study-plan/)
---

## **Lesson 1**

### What is SASS?
- **SASS** stands for Syntactically Awesome Style Sheets.
- SASS is a preprocessor that allows us to write code with SASS syntax, and using a compiler we can compile it to CSS code.
- SASS is extension for CSS.

### Why we use SASS?
- With SASS we can save time, reduce errors, and structure our files.
- Whit SASS we can use the programming languages features.

### What are SASS features?
- Variables
- Built-in functions and writing our custom functions
- Loop with loop we can create many classes, e.g. to create a classes that represent font size from 10px to 100px with normal CSS we must write the manually, but using SASS we can do that in one loop.
- Extend with this feature we can reuse a defined class in another class.
- Control flow with can use if statement to control something specific. 
- Advanced structure

---

## **Lesson 2**

### Websites to try SASS
- [sassmeister](https://www.sassmeister.com/)
- [code pen](https://www.codepen.io)
### How to compile SASS?
- We can compile the SASS by using an extension in VS Code called **Live SASS compiler**.
- With desktop applications Koala and Prepros 
- With npm packages like SASS.


### Ways to write SASS
- **SCSS**: Written like CSS with curly braces.
- **SASS**: Written like Python language depending on indentation. 

---

## **Lesson 3**

#### **_NOTES:_** During working with the SASS files, this stage called developing. But when the files compiled and compressed to CSS files, these files called production files.

### How to import SASS files?
- To import SASS files we use the ( @use ) method to import the files, the ( @import ) method deprecated.

### How to structure your project SASS files?
- Folder for the layout files contain the global file.
  - The global file contain the rules for the whole website e.g. *, body, button, a, ...
  - The files prefixed with the (_) underscore prevent the compiler from compiling the file.