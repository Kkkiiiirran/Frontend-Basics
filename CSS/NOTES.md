[Google Fonts](fonts.google.com)

[Text-Align](https://developer.mozilla.org/en-US/docs/Web/CSS/text-align)
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

# External CSS syntax

```
  <html>
    <head>  
      <title>hello</title>
      <link rel="stylesheet" href="style.css">
    </head>
   </html>
```

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


<hr>

### Sizes of Texts

**1px**: 1/96th of an inch

**1pt**: 1/72th of an inch -- _12pt = calibari 12 size in word_

**1em**: 100% of parent

**1rem**: 100% root

**font-weight**: normal || bold || lighter _-100_ || bolder _+100_

**font-family**: sans serif, serif, 

syntax:
```font-family: helvetica, sans serif```

```font-family: "Times of India", serif```

**Text-align**:centre || left || right || start || end || justify 

**Text-align-last**: auto || centre || left || right || start || end || justify _aligns the last line of the text_

<hr>

### BOX MODEL
**Height**: 10px  _in pixels_ || 100% _in percentage_

**Width**: 10px _in pixels_ || 100% _in percentage_

**Border**: the outline of a the box in which resides an element

#### Syntax:
            
                      border: value style color

#### Example
           
                      border: 10px solid black

**border-top** || **border-bottom** || **border-right** || **border-left**

**border-width**

#### Syntax:
          
                     border-width: top right bottom left

                     border-width: top_and_bottom  right_and_left

#### Example
          
                    border-width: 10px 20px 30px 40px

                    border-width: 10px 20px
                    
**padding**: outside the element tag but inside the border
            the dimensions of the element box remains unchanged

#### Syntax:
          
                    padding: top right bottom left

                    padding: top_and_bottom  right_and_left

#### Example
          
                    padding: 10px 20px 30px 40px

                    padding: 10px 20px

**margin**: outside the borders

#### Syntax:
          
                    margin: top right bottom left

                    margin: top_and_bottom  right_and_left

#### Example
          
                    margin: 10px 20px 30px 40px

                    margin: 10px 20px

#### Example: 
![image](https://github.com/Kkkiiiirran/Frontend-Basics/assets/136697603/b94df0cf-a3ca-48c4-a2e4-808c3fdf7112)


### div

<div>
  <p>I am a element in a div element</p>
  <h2>I am another element in the same div element</h2>
</div>

#### Centering a div horizontally

```width: 50%;
   margin-left: 25%;
```

```height: 50%;
   margin-top: 25%;
```

<hr>

### CSS RULES
![image](https://github.com/Kkkiiiirran/Frontend-Basics/assets/136697603/6c412d01-e42c-4b06-95b1-e9390ef2d525)

### Combining CSS Selectors
#### Group Rule
##### Syntax:

                    selector, selector {
                    color: red; }


##### Example
          
                    div, p {
                    color: purple;}

#### Child Rule

##### Syntax:

                    selector > selector {
                    color: red; }


##### Example
          
                    .box > p {
                    color: purple;}

#### Descendent Rule

##### Syntax:

                    selector selector {
                    color: red; }


##### Example
          
                    .box li {
                    color: purple;}
                    
#### Chain Rule

##### Syntax:

                    selectorselector {
                    color: red; }


##### Example
          
                    li.box.innerbox {
                    color: purple;}


#### Combining combined selectors

##### Syntax:

                    selector selectorselector {
                    color: red; }


##### Example
          
                    p box.innerbox {
                    color: purple;}

<hr>                

### Positioning

#### Static
#### Relative
#### Absolute
#### Fixed

<hr>

### Display

#### Block
Let's you alter the height and width but does not allow any other element to be in the same line.

#### Inline
Does not let you alter the height and width but allows any other element to be in the same line.

#### Inline-block
Allows both, to alter height and width as well allows other elements to be in same line.

#### none
hides the element

### [Example](https://appbrewery.github.io/css-display/)

<hr>

#### float
          img {
          float: left || right }
will shift the image left and right whcih allows the text below to take up space adjacent to the image.
if you do not wish certain text to take the adjacent space, just use

#### clear

        img {
        float: left || right}
        footer {
        clear: left || right || both }
  

                    

            
                    
