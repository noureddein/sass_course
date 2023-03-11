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

---

## **Lesson 4**

### Variables
- Variables in SASS works like any programming language
  - Global variables
  - Local variables
- In CSS the property take the name of the variable not the value.
```CSS
:root{
    --main-color: red
}

.header{
    background-color: var(--main-color);
}
```
- In SASS the property take the value of the variable.

```CSS
// Before compile

$alt_color: green;

.header{
    background-color: $alt_color;
}
```

```CSS
// After compile

.header{
    background-color: green;
}
```

- To overwrite a global variable from a local scop we use the !global flag.
- To import a file contain the variables:
  - ( @use './SASS/variables/_colors.scss' as *; ) then we can use the variable.
  - ( @use './SASS/variables/_colors.scss'; ) then we can use the variable $colors.$var_name.

---

## **Lesson 5**

- SASS have a feature called nesting its like object to define the properties.
```CSS
.parent{
    font-size: 16px;
    .child{
        font-size: 16px;
        .grand-child{
            font-size: 16px;    
        }
    }
}
```

- Direct element
```CSS
.parent > {
    .child {
        font-size: 10px;
    }

    .test {
        padding: 5px;
    }
}
```
- Grouping
```CSS
.parent-one,
.parent-two {
    padding: 20px;
    .child {
        padding: 10px;
    }
}
```

- Multi class for the same element

```CSS
.box{
    .title{
        font-size: 14px;
    }

    .description{
        font-size: 12px;
    }

    &.red{
        background-color: red;
    }

    &.green{
        background-color: green;
    }
}
```
- Pseudo class
```CSS
.box{
    .title{
        font-size: 14px;
    }

    .description{
        font-size: 12px;
    }

    &.red{
        background-color: red;
    }

    &.green{
        background-color: green;
    }

    /*  Pseudo class */
    &:hover{
        background-color: green;
    }
}

```