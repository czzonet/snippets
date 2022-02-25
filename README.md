```js
{
  // Place your global snippets here. Each snippet is defined under a snippet name and has a scope, prefix, body and
  // description. Add comma separated ids of the languages where the snippet is applicable in the scope field. If scope
  // is left empty or omitted, the snippet gets applied to all languages. The prefix is what is
  // used to trigger the snippet and the body will be expanded and inserted. Possible variables are:
  // $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders.
  // Placeholders with the same ids are connected.
  // Example:
  // "Print to console": {
  // 	"scope": "javascript,typescript",
  // 	"prefix": "log",
  // 	"body": [
  // 		"console.log('$1');",
  // 		"$2"
  // 	],
  // 	"description": "Log output to console"
  // }
  "const": {
    "scope": "javascript,typescript,typescriptreact,javascriptreact",
    "prefix": "ct",
    "body": ["const "],
    "description": "Shotcut for const"
  },

  "reactFunctionalComponent": {
    "scope": "typescriptreact",
    "prefix": "trfc",
    "body": [
      "import React from 'react'",
      "",
      "export const ${1:${TM_FILENAME_BASE}}: React.FC = () => {",
      "\treturn (",
      "\t\t<div>",
      "\t\t\t$0",
      "\t\t</div>",
      "\t)",
      "}",
      ""
    ],
    "description": "Creates a React Functional Component with ES7 module system"
  },
  "reactHook": {
    "scope": "typescript",
    "prefix": "trh",
    "body": [
      "export const ${1:${TM_FILENAME_BASE}} = () => {",
      "\treturn {}",
      "}",
      ""
    ],
    "description": "Creates a React Hook with ES7 module system"
  },
  "test": {
    "scope": "typescript,typescriptreact",
    "prefix": "test",
    "body": [
      "describe('${1:${TM_FILENAME_BASE}}', () => {",
      "\tit('should',()=> {",
      "})});",
      ""
    ],
    "description": "Creates a test"
  },
  "todo": {
    "scope": "typescript,typescriptreact",
    "prefix": "TODO",
    "body": ["TODO:"],
    "description": "Creates a TODO"
  }
}

```
