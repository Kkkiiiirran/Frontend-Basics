# Inline CSS syntax
`<h1 style="color: red;">Hey</h1>`

<hr>

# Internal CSS syntax
```
  <html>
    <head>  
      <title>hello</title>
      <style> h1 {color: blue;} </style>
    </head>
   </html>
```
<hr>

## Selectors in CSS

### Element Selector

Syntax      :    `h1 { attribute: value;}`
> **Note** applies the same formatting to all the elements of that kind.

#### Example
```
  <h1>Hey</h1>
  <h1>Hey 1</h1>
  <h1>Hey 2</h1>
```

If we apply `h1 { color: red; }` to the above code.

All the h1 elements in the document will turn red.

<hr>

### Class Selector
syntax      :      `.classname {attribute: value;}`
> **Note** applies the same formatting to all the elements with the same classname as selected above.

#### Example
<div class="new-class>
  <h2>Great</h2>
  <h2>A great evening</h2> 
</div>

if we apply `.new-class {color: red;}`

All the elements in the document with _new-class_ will turn red.

<hr>

### ID Selector
syntax    :        `#id-name {attribute: value;}`
> **Note** Id is unique.
> An Id selector applies the formatting to only one element with that Id-name


#### Example
```
    <div class="new-class>
    <h2>Great</h2>
    <h2 id="new-id">A great evening</h2>
    <h2>sunshine</h2>
    </div>
```

if we apply #new-id {color: red;} to the above text,
the element h2 with the id name _new-id_ will turn red

<hr>

### Attribute Selector

syntax      :      `element(x)[attribute(y)] {attribute: value;}`
> **Note** an attribute selector will apply formatting to all the elements (x) with the attribute (y).

#### Example 1
```<button type="submit">Click Me</button>
  <button type="reset">Click Me</button>
  <button type="submit">Click Me</button>
  <button type="submit">Click Me</button>
  <button type="reset">Click Me</button>
  <button type="submit">Click Me</button>
```

if we apply button[submit] {formtarget: "_blank";} <!---formtarget="blank" directs the user to a new window when the button is clicked--->
then all the button with the type _submit_ will direct the user to a new window when clicked.

#### Example 2
```
    <p draggable="true">hey</p>
    <p draggable="true">hello</p>
    <p draggable="false">hi</p>
```

if we apply p[draggable="false"] {color:red;} to the above code then olny the last p will change it's colour to red 

<hr>

### Universal Selector
syntax    :   `*{color:red}`
> **Note** this selector will apply the formatting to all the elements in the document.

#### Example 1

```     <p draggable="true">hey</p>
        <p draggable="true">hello</p>
        <p draggable="false">hi</p>
        <button type="submit">Click Me</button>
        <button type="reset">Click Me</button>
        <button type="submit">Click Me</button>
        <button type="submit">Click Me</button>
        <button type="reset">Click Me</button>
        <button type="submit">Click Me</button>
        <h1>Hey</h1>
        <h1>Hey 1</h1>
        <h1>Hey 2</h1>
        <div class="new-class>
        <h2>Great</h2>
        <h2>A great evening</h2> 
    </div>
```

if we apply *{color:red;}
all the elements in the document will turn red.
