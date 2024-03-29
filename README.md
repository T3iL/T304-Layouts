# 04 - Layouts

## -------INFO

1. CSS - Block, Inline, Inline-block
2. CSS - Box model
3. CSS - Floats
```html
...
    <style>
        *{
            margin:0;
            padding:0;
            box-sizing:border-box;
        }
        html,body,#container{
            height:100%;
        }
        #container{
            width:400px;
            margin:auto;
        }
        #container > div {
            border:1px solid;
        }
        #left{
            height:80%;
            width:30%;
            float:left;
        }
        #right{
            height:80%;
            width:70%;
            float:right;
        }
        .clear{
            clear:both;
        }
    </style>
...
    <div id="container">
        <div id="left">LEFT</div>
        <div id="right">RIGHT</div>
        <div class="clear">FOOTER</div>
    </div>
```

clearfix pseudo element:
```css
.clearfix:after {
  content: "";
  display: table;
  clear: both;
}
```

6. CSS - Flex
```html
...
    <style>
        *{
            margin:0;
            padding:0;
            box-sizing:border-box;
        }
        html,body,#container{
            height:100%;
        }
        #container{
            display:flex;
            flex-direction: row-reverse;/* row | column */
            flex-wrap:wrap;
            justify-content: center; /* flex-start | flex-end | space-between | space-around | space-evenly */
            align-items: center; /* stretch | flex-start | flex-end */
            align-content: center; /* flex-start | flex-end | | space-between | space-around | space-evenly | stretch */
            gap:10px;
        }
        #container > div{
            border:1px solid;
            width:100px;
            height:100px;
        }
    </style>
...
    <div id="container">
        <div>1</div>
        <div>2</div>
        <div>3</div>
        <div>4</div>
        <div>5</div>
    </div>
...
```
5. CSS - Grid
```html
...
    <style>
        #container{
            display:grid;
            grid-template-columns: 1fr 3fr 1fr;
            grid-template-rows: 1fr 5fr;
        }
        #container > div{
            border:1px solid;
        }
        #d1{
            grid-column-start: 1;
            grid-column-end: 4;
            grid-row-start: 2;
        }
    </style>
...
    <div id="container">
        <div id="d1">1</div>
        <div id="d2">2</div>
        <div id="d3">3</div>
        <div id="d4">4</div>
        <div id="d5">5</div>
        <div id="d6">6</div>
        <div id="d6">7</div>
    </div>
```
6. CSS - positions
7. CSS - Transform



https://miroslawzelent.pl/kurs-css/

https://htmlcheatsheet.com/css/

[Block, Inline, and Inline-Block explained | CSS Tutorial](https://youtu.be/x_i2gga-sYg)

[Floats, Flexbox, Grid? The progression of CSS layouts](https://youtu.be/R7gqJkdc5dM)

[CSS-Tricks Float](https://css-tricks.com/almanac/properties/f/float/) |
[CSS-Tricks Flex](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) |
[CSS-Tricks Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

```
ZADANIA

T30501. Przygotuj layout przedstawiony na obrazie Layout_07 w dwóch wersjach: 

- tylko przy pomocy float
- tylko przy pomocy flex
```
![Layout_07](/Layout_02.PNG)
![Layout_07](/Layout_07.jpg)

ZADT30402 - Przygotuj w programie graficznym schemat layoutu dziesięciu wybranych stron z katalogu Layout (link poniżej).

https://drive.google.com/drive/folders/13lyoR2wH2LrDdUcLWojNBxd6DyDRQ_e_?usp=sharing



### --------Links
https://github.com/T3iL/T304-Layouts

GOOGLE DRIVE: https://drive.google.com/drive/folders/1OqTcjwr_qAdTPO-dThxUOd3ooTTOlzgp?usp=sharing

https://www.w3.org | https://validator.w3.org | https://www.php.net/manual/en/
### --------Repositiories
https://www.w3schools.com | https://stackoverflow.com | https://css-tricks.com |
### --------On line editors
https://codepen.io/ | https://codesandbox.io/ | https://jsfiddle.net/ | nicepage.com
### ---------Assets
https://cdnjs.com/ | https://fontawesome.com | http://fontello.com/ | https://fonts.google.com/ | https://www.flaticon.com/
### ---------Stock Img
https://www.pexels.com/ | https://unsplash.com | https://pixabay.com
### ---------Tuts
https://www.youtube.com/watch?v=1Rs2ND1ryYc
https://www.youtube.com/watch?v=J35jug1uHzE
https://www.youtube.com/watch?v=ieTHC78giGQ
### ---------License
[MIT](https://choosealicense.com/licenses/mit/)
