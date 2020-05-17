# Syntaxs


```
element    = | div attributes children
             | str "text"
             | img "img-name"
             
attribute  = | Class "class-name"
             | Visible (true | false)
             
             
attributes = attribute list
children   = element list

```

# Examples

```

div [Class "main-panel"] [
    str "Hello world"    
]

```
