# AdvPL/TLPP Code Snippets for VS Code

A comprehensive collection of code snippets for **AdvPL** (Advanced Protheus Language) and **TLPP** (TOTVS Language Plus Plus) development in Visual Studio Code.

## 📋 Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [How to Use](#how-to-use)
- [Available Snippets](#available-snippets)
- [Snippet Categories](#snippet-categories)
- [Features](#features)
- [Examples](#examples)
- [Customization](#customization)
- [Contributing](#contributing)

## 🎯 Overview

This snippet collection provides **70+ ready-to-use code templates** for AdvPL/TLPP development, covering:

- Variable declarations with proper Hungarian notation
- Control flow statements and loops
- Function and method declarations with Protheus.doc documentation
- Object-oriented programming constructs
- Web services (WSService, WSMethod, WSStruct)
- Embedded content blocks (JavaScript, TypeScript, HTML, CSS, JSON, XML)
- Preprocessor directives
- Complete program and class templates

## 🚀 Installation

### Method 1: Manual Installation
1. Copy the `advpl_complete_snippets.json` file to your VS Code snippets folder:
   - **Windows**: `%APPDATA%\Code\User\snippets\`
   - **macOS**: `~/Library/Application Support/Code/User/snippets/`
   - **Linux**: `~/.config/Code/User/snippets/`

2. Rename the file to `advpl.json` or `tlpp.json`

### Method 2: Via Extension (if part of TOTVS extension)
The snippets are automatically available when using the TOTVS Developer Studio extension.

## 💡 How to Use

1. **Type the snippet prefix** (e.g., `function`, `class`, `if`)
2. **Press Tab** when the snippet appears in the autocomplete list
3. **Navigate between placeholders** using Tab
4. **Fill in your specific values** at each placeholder
5. **Press Escape** to exit snippet mode

### Quick Example
```
Type: function + Tab
Result: Complete function template with documentation
```

## 📚 Available Snippets

### 🔧 Variable Declarations
| Prefix | Description | Output |
|--------|-------------|--------|
| `local` | Local variable | `Local cVariable := "value"` |
| `localas` | Typed local variable | `Local cVariable AS Character` |
| `private` | Private variable | `Private cVariable := "value"` |
| `static` | Static variable | `Static nVariable := 0` |
| `public` | Public variable | `Public cVariable := "value"` |

### 🔀 Control Flow
| Prefix | Description | Output |
|--------|-------------|--------|
| `if` | Basic if statement | `If condition ... EndIf` |
| `ifelse` | If-else statement | `If...Else...EndIf` |
| `ifelseif` | If-elseif-else | `If...ElseIf...Else...EndIf` |
| `docase` | Do case statement | `Do Case...EndCase` |

### 🔄 Loops
| Prefix | Description | Output |
|--------|-------------|--------|
| `for` | Basic for loop | `For nI := 1 To 10...Next` |
| `forstep` | For loop with step | `For nI := 1 To 100 Step 5` |
| `while` | While loop | `While condition...End` |
| `exit` | Exit loop | `Exit` |
| `loop` | Continue loop | `Loop` |

### ⚙️ Functions
| Prefix | Description | Output |
|--------|-------------|--------|
| `function` | Function with docs | Complete function template |
| `staticfunc` | Static function | Static function template |
| `main` | Main function | Main function entry point |
| `user` | User function | User function template |

### 🏗️ Object-Oriented Programming
| Prefix | Description | Output |
|--------|-------------|--------|
| `class` | Class declaration | Complete class structure |
| `classfrom` | Class with inheritance | Class extending parent |
| `method` | Method implementation | Method with documentation |
| `constructor` | Constructor method | Class constructor |
| `classtemplate` | Complete class | Full class with methods |

### 🌐 Web Services
| Prefix | Description | Output |
|--------|-------------|--------|
| `wsservice` | Web service | WSService declaration |
| `wsmethod` | WS method | WSMethod implementation |
| `wsstruct` | WS structure | WSStruct declaration |
| `wsclient` | WS client | WSClient declaration |
| `wsrestful` | RESTful service | WSRestful declaration |

### 📄 Embedded Content
| Prefix | Description | Output |
|--------|-------------|--------|
| `beginjs` | JavaScript block | BeginContent...JavaScript |
| `begints` | TypeScript block | BeginContent...TypeScript |
| `beginhtml` | HTML block | BeginContent...HTML |
| `begincss` | CSS block | BeginContent...CSS |
| `beginjson` | JSON block | BeginContent...JSON |
| `beginxml` | XML block | BeginContent...XML |

### 🔧 Preprocessor
| Prefix | Description | Output |
|--------|-------------|--------|
| `include` | Include directive | `#Include "file.ch"` |
| `define` | Define directive | `#Define CONSTANT value` |
| `ifdef` | Conditional compilation | `#IfDef...#EndIf` |
| `ifdefelse` | Ifdef with else | `#IfDef...#Else...#EndIf` |
| `ifndef` | Ifndef directive | `#IfNDef...#EndIf` |

### 🎨 UI & Database
| Prefix | Description | Output |
|--------|-------------|--------|
| `definedialog` | Dialog definition | Complete dialog setup |
| `select` | Select area | `Select Area` |
| `use` | Use table | `Use Table` |
| `default` | Default parameter | `Default param := value` |

### 📦 Complete Templates
| Prefix | Description | Output |
|--------|-------------|--------|
| `program` | Complete program | Full program template |
| `classtemplate` | Complete class | Full class with methods |

## ✨ Features

### 🎯 Smart Placeholders
- **Tab stops**: Navigate through editable sections
- **Default values**: Meaningful defaults for quick development
- **Linked placeholders**: Same values auto-update across the snippet

### 📋 Choice Lists
Some snippets include dropdown menus for common options:
```json
"${2|Character,Numeric,Logical,Date,Array,Object,CodeBlock,Json,Variant|}"
```

### 🔄 Auto Variables
- `$TM_USERNAME`: Current username
- `$CURRENT_DATE`: Current date
- `$CURRENT_MONTH`: Current month
- `$CURRENT_YEAR`: Current year

### 📖 Protheus.doc Integration
All function snippets include proper documentation format:
```advpl
/*/{Protheus.doc} FunctionName
    Function description
    @type  Function
    @author username
    @since 02/07/2025
    @version 1.0
    @param param, type, description
    @return return_var, return_type, return_description
/*/
```

## 🔥 Examples

### Function Example
**Input**: `function` + Tab
**Output**:
```advpl
/*/{Protheus.doc} FunctionName
    Function description
    @type  Function
    @author YourUsername
    @since 02/07/2025
    @version 1.0
    @param param, type, description
    @return return_var, return_type, return_description
/*/
Function FunctionName(param)
    Local cResult := ""
    
    
    
Return cResult
```

### Class Example
**Input**: `class` + Tab
**Output**:
```advpl
/*/{Protheus.doc} ClassName
    Class description
    @author YourUsername
    @since 02/07/2025
    @version 1.0
/*/
Class ClassName
    Data cProperty
    Data nValue
    
    Method New() Constructor
    Method MethodName()
EndClass
```

### Web Service Example
**Input**: `wsservice` + Tab
**Output**:
```advpl
WSService ServiceName Description "Service description"
    WSData cParam AS String
    WSData nValue AS Integer
    
    WSMethod MethodName Description "Method description"
EndWSService
```

### Embedded JavaScript Example
**Input**: `beginjs` + Tab
**Output**:
```advpl
BeginContent Var cJSCode As JavaScript
    function myFunction() {
        console.log("Hello from JavaScript");
        return %cAdvPLVariable%;
    }
EndContent
```

## 🎨 Customization

### Modifying Snippets
1. Open VS Code settings (`Ctrl+,`)
2. Search for "snippets"
3. Click "Edit in settings.json"
4. Modify existing snippets or add new ones

### Adding Custom Snippets
```json
{
    "My Custom Snippet": {
        "prefix": "mycustom",
        "body": [
            "// Your custom code here",
            "${1:placeholder}"
        ],
        "description": "My custom snippet description"
    }
}
```

### Snippet Variables
You can use these VS Code variables in your snippets:
- `$TM_SELECTED_TEXT`: Currently selected text
- `$TM_CURRENT_LINE`: Current line content
- `$TM_CURRENT_WORD`: Current word under cursor
- `$TM_LINE_INDEX`: Line number (zero-based)
- `$TM_LINE_NUMBER`: Line number (one-based)
- `$TM_FILENAME`: Current filename
- `$TM_FILENAME_BASE`: Filename without extension
- `$TM_DIRECTORY`: Directory of current file
- `$TM_FILEPATH`: Full file path

## 🛠️ Best Practices

### Using Hungarian Notation
Follow TOTVS conventions for variable naming:
- `c` for Character/String variables
- `n` for Numeric variables
- `l` for Logical/Boolean variables
- `d` for Date variables
- `a` for Array variables
- `o` for Object variables
- `b` for Block/CodeBlock variables

### Documentation Standards
Always use the Protheus.doc format for functions:
```advpl
/*/{Protheus.doc} FunctionName
    Brief description
    @type Function
    @author Author Name
    @since DD/MM/YYYY
    @version 1.0
    @param paramName, paramType, paramDescription
    @return returnVar, returnType, returnDescription
    @example
    result := FunctionName("example")
    @see RelatedFunction
/*/
```

### Code Organization
- Use static functions for internal operations
- Keep functions focused and single-purpose
- Include proper error handling
- Use meaningful variable and function names

## 🤝 Contributing

### Adding New Snippets
1. Follow the existing naming conventions
2. Include proper documentation
3. Test the snippet thoroughly
4. Add to the appropriate category

### Snippet Format
```json
{
    "Snippet Name": {
        "prefix": "shortcut",
        "body": [
            "line 1",
            "line 2 with ${1:placeholder}",
            "line 3"
        ],
        "description": "Brief description of what this snippet does"
    }
}
```

### Guidelines
- Use meaningful prefixes (3-10 characters)
- Include helpful placeholders
- Provide clear descriptions
- Follow AdvPL/TLPP syntax conventions
- Test with different VS Code themes

## 📝 License

This snippet collection is part of the TOTVS Developer Studio extension and follows the same license terms.

## 🔗 Related Resources

- [AdvPL/TLPP Documentation](link-to-docs)
- [TOTVS Developer Studio Extension](link-to-extension)
- [Protheus Development Guide](link-to-guide)
- [TLPP Language Reference](link-to-reference)

---

**Happy Coding with AdvPL/TLPP! 🚀**

For issues, suggestions, or contributions, please refer to the main extension repository.
