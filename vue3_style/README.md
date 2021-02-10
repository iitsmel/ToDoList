# kotlin
# vue

## problem encountered and solved
### [Syntax Error: TypeError: this.getOptions is not a function.](https://stackoverflow.com/questions/66082397/typeerror-this-getoptions-is-not-a-function)
- "Similar to what @KostDM said, in my case it seems like sass-loader@11.0.0 doesn't work with vue@2.6.12. I installed sass-loader@10.1.1 and it worked like a charm again." [name=D_Pain]
<br>

- npm i -D sass-loader@10
<br>

### The component has been registered but not used .
- put '  /* eslint-disable vue/no-unused-components */  ' in js
<br>

### [The template root requires exactly one element.](https://stackoverflow.com/questions/64867504/vue-3-the-template-root-requires-exactly-one-element-eslint-plugin-vue)
- You can solve this by doing '  F1>Preferences:Open Settings (JSON) '
- paste
    - "vetur.validation.template": false,
    - "vetur.validation.script": false,
    - "vetur.validation.style": false,
    - [name=MikeOttink]

### [Rule can only have one resource source (provided resource and test + include + exclude)](https://stackoverflow.com/questions/64373393/error-rule-can-only-have-one-resource-source-provided-resource-and-test-incl)
- Type in the commands below. It works for me.
- npm uninstall webpack
- npm install webpack@^4.0.0 --save-dev
- [name=Cvincent]