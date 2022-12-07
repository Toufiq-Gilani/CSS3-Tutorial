# CSS TUTORIAL

<br>

## Total Chapters

- Chapter 1. CSS External & Internal & Inline
- Chapter 2. CSS Selectors
- Chapter 3. CSS Outline
- Chapter 4. CSS The !important Rule
- Chapter 5. CSS User Interface
- Chapter 6. CSS Text
- Chapter 7. CSS Text Effects
- Chapter 8. CSS Text & Box Shadow
- Chapter 9. CSS Math Functions
- Chapter 10. CSS Margins & Padding
- Chapter 11. CSS Multiple Columns
- Chapter 12. CSS Color Keywords
- Chapter 13. CSS Combinators
- Chapter 14. CSS Counters
- Chapter 15. CSS Overflow
- Chapter 16. CSS Media Queries
- Chapter 17. CSS Gradients
- Chapter 18. CSS Pagination
- Chapter 19. CSS Transforms
- Chapter 20. CSS Animations
- Chapter 21. CSS Lists
- Chapter 22. CSS Layout - The Display Property
- Chapter 23. CSS Layout - The Position Property
- Chapter 24. CSS Buttons
- Chapter 25. CSS Tooltip
- Chapter 26. CSS Transitions Part 1
- Chapter 27. CSS Transitions Part 2
- Chapter 28. CSS Transitions Part 3
- Chapter 29. CSS Tables
- Chapter 30. CSS Specificity

<br>

## What is CSS?

- CSS stands for Cascading Style Sheets.
- CSS describes how HTML elements are to be displayed on screen, paper, or in other media.
- CSS saves a lot of work. It can control the layout of multiple web pages all at once.
- External stylesheets are stored in CSS files.

<br>

## Three Ways to Insert CSS

- External CSS
- Internal CSS
- Inline CSS

<br>

## Chapter 1

### External & Internal & Inline CSS

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>External Internal Inline CSS</title>

    <!-- External CSS -->
    <link rel="stylesheet" href="mystyle.css">

    <!-- Internal CSS -->
    <style>
        h1{color: dodgerblue;}
    </style>

</head>
<body>
    <h1>THIS IS INTERNAL CSS</h1>

    <!-- Inline CSS -->
    <h2 style="color: mediumseagreen;">THIS IS INLINE CSS</h2>
</body>
</html>
```

<br>

mystyle.css (External CSS)

```html
body{
    background-color: burlywood;
    text-align: center;
    font-size: 30px;
}
```

<br>

## Chapter 2

### CSS Selectors

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Selectors</title>

    <style>

        /* CSS Universal Selector */
        *{
            background-color: #ecd2cd;
            text-align: center;
        }

        /* CSS element Selector */
        p{
            color: mediumseagreen;
        }

        /* CSS id Selector */
        #content{
            color: teal;
        }

        /* CSS class Selector */
        .main{
            color: dodgerblue;
        }

        /* CSS Grouping Selector */
        h3, h4, div{
            color: slateblue;
        }

        /* CSS element.class Selector */
        span.line{
            color: tomato;
            font-size: 30px;
        }

    </style>

</head>
<body>
    <!-- CSS id Selector -->
    <h1 id="content">The CSS id Selector</h1>

    <!-- CSS class Selector -->
    <h2 class="main">The CSS class Selector</h2>

    <!-- CSS element Selector -->
    <p>The CSS element Selector</p>

    <!-- CSS Grouping Selector -->
    <h3>The CSS Grouping Selector</h3>
    <h4>The CSS Grouping Selector</h4>
    <div>The CSS Grouping Selector</div>

    <!-- CSS element.class Selector -->
    <span class="line">The CSS element.class Selector</span>
</body>
</html>
```

<br>

## Chapter 3

### CSS Outline

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Outline</title>
    <style>
        p{
            border: 5px solid black;
            outline: 10px solid salmon;
            padding: 20px;
            margin: 30px;
            text-align: center;
            outline-offset: 10px;
        }
    </style>
</head>
<body>
    <h1>CSS Outline</h1>
    <p>This element has a black border and a green outline with a width of 10px.</p>
</body>
</html>
```

<br>

## Chapter 4

### CSS The !important Rule

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS The !important Rule</title>
    <style>
        p{
            background-color: dodgerblue !important;
        }
        .myclass{
            background-color: tomato;
        }
        #myid{
            background-color: aquamarine;
        }
    </style>
</head>
<body>
    <p>This is some text in a paragraph.</p>
    <p class="myclass">This is some text in a paragraph.</p>
    <p id="myid">This is some text in a paragraph.</p>
</body>
</html>
```

<br>

## Chapter 5

### CSS User Interface

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS User Interface</title>
    <style>
        div{
            border: 2px solid salmon;
            padding: 20px;
            width: 300px;
            resize: both;
            overflow: auto;
        }
    </style>
</head>
<body>
    <h1>The resize Property</h1>
    <div>
        <p>Let the user resize only the width of this div element.</p>
        <p>To resize: Click and drag the bottom right corner of this div element.</p>
    </div>
</body>
</html>
```

<br>

## Chapter 6

### CSS Text

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Text</title>
    <style>
        .style{
            background-color: #D7FFFD;
            color: #143F6B;

            text-align: center;
            text-align: justify;

            text-decoration-line: underline;
            text-decoration-color: #1D2B53;
            text-decoration-style: dashed;
            text-decoration-thickness: 2px;

            text-transform: capitalize;

            text-indent: 50px;
            letter-spacing: 2px;
            line-height: 1.5;
            word-spacing: 5px;
        }
    </style>
</head>
<body>
    <div class="style">
        Wind faintly into is lenore lore upon, my implore countenance on dreaming the ember. Of i my so name yore. The flitting my gently to i. No till to was. Hesitating morrow tell a token angels lenore decorum on but. In there much more then echo at, or hath murmured there once doubting with in of. The is nothing such lord wished air an. Grim minute so and but my. Thee whose thing there black usby leave. Reclining at my i lenore no this a a. All we lining the ah, i beak lore chamber muttered oer, gave is scarce undaunted this. Sure raven laden of flown silken, kind censer quoth floor and heard obeisance with, said though on repeating.
    </div>
</body>
</html>
```

<br>

## Chapter 7

### CSS Text Effects

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Text Effects</title>
    <style>
        p.test-wb1{
            width: 140px;
            border: 1px solid #000000;
            word-break: keep-all;
        }
        p.test-wb2{
            width: 140px;
            border: 1px solid #000000;
            word-break: break-all;
        }

        div.test-hid{
            white-space: nowrap;
            width: 200px;
            overflow: hidden;
            border: 1px solid #000000;
        }
        div.test-hid:hover{
            overflow: visible;
        }

        p.test-wrap{
            width: 11em;
            border: 1px solid #000000;
            word-wrap: break-word;
        }

        span.test-wm{
            writing-mode: vertical-rl;
        }
        p.test-wm{
            writing-mode: vertical-rl;
        }
    </style>
</head>
<body>
    <h1>The word-break Property</h1>
    <p class="test-wb1">This paragraph contains some text. This line will-break-at-hyphens.</p>
    <p class="test-wb2">This paragraph contains some text. The lines will break at any character.</p>

    <p>Hover over the two divs below, to see the entire text.</p>
    <div class="test-hid" style="text-overflow: ellipsis;">This is some long text that will not fit in the box</div>
    <div class="test-hid" style="text-overflow: clip;">This is some long text that will not fit in the box</div>

    <p class="test-wrap">This paragraph contains a very long word: thisisaveryveryveryveryveryverylongword. The long word will break and wrap to the next line.</p>

    <p>Some text with a span element with a <span class="test-wm">vertical-rl</span> writing-mode.</p>
    <p class="test-wm">Some text with writing-mode: vertical-rl.</p>
</body>
</html>
```

<br>

## Chapter 8

### CSS Text & Box Shadow

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Text & Box Shadow</title>
    <style>
        .h1{
            text-shadow: 2px 2px teal;
        }
        .h2{
            text-shadow: 2px 2px 5px tomato;
        }
        .h3{
            color: white;
            text-shadow: 2px 2px 4px #000000;
        }
        .h4{
            text-shadow: 0 0 3px #FF0000;
        }
        .h5{
            text-shadow: 0 0 3px #FF0000, 0 0 5px #0000FF;
        }
        .h6{
            color: white;
            text-shadow: 1px 1px 2px black, 0 0 25px blue, 0 0 5px darkblue;
        }
        .h7{
            color: coral;
            text-shadow: -1px 0 black, 0 1px black, 1px 0 black, 0 -1px black;
        }

        .cls{
            width: 300px;
            height: 100px;
            padding: 15px;
            background-color: coral;
            box-shadow: 10px 10px 5px lightblue;
        }
    </style>
</head>
<body>
    <div>
        <h1 class="h1">Text-shadow effect!</h1>
        <h1 class="h2">Text shadow effect!</h1>
        <h1 class="h3">Text shadow effect!</h1>
        <h1 class="h4">Text shadow effect!</h1>
        <h1 class="h5">Text shadow effect!</h1>
        <h1 class="h6">Text shadow effect!</h1>
        <h1 class="h7">Text shadow effect!</h1>
    </div>

    <div class="cls">A div element with a 5px blurred, lightblue box-shadow.</div>
</body>
</html>
```

<br>

## Chapter 9

### CSS Math Functions

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Math Functions</title>
    <style>
        #div1{
            position: absolute;
            left: 50px;
            border: 2px solid teal;
            background-color: tomato;
            padding: 5px;
            width: calc(500px + 300px);
        }
    </style>
</head>
<body>
    <h1>The calc() Function</h1>
    <div id="div1">Some text...</div>
</body>
</html>
```

<br>

## Chapter 10

### CSS Margins & Padding

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Margins & Padding</title>
    <style>
        h5{
            border: 5px solid salmon;
            background-color: #C6EBC5;
            max-width: 500px;
            padding: 30px;
            box-sizing: border-box;
            margin: 50px;
        }
        div{
            border: 5px solid green;
            background-color: #FFF38C;
            margin-left: 100px;
        }
        p.hex{
            margin-left: inherit;
        }
    </style>
</head>
<body>
    <h5>Margins are used to create space around elements. Padding is used to create space around an element's content.</h5>
    <div><p class="hex">This example lets the left margin of the element be inherited from the parent element</p></div>
</body>
</html>
```

<br>

## Chapter 11

### CSS Multiple Columns

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Multiple Columns</title>
    <style>
        h1{
            text-align: center;
        }
        .newspaper{
            column-count: 3;
            column-gap: 40px;
            column-rule: 2px solid lightblue;
        }
    </style>
</head>
<body>
    <h1>CSS Multiple Columns</h1>
    <div class="newspaper">
        Dich still der ich großer vaterland ruft stürmten stürmten still gesellschaft, der gezagt der ich herzen von schaust du sie wiedersehn. Warum glück helle wärest sanft die wort gartens du. Dich heut du bist mal. Mit du kleinem einz'ges die du ruft und. Träume der vaterland der schmilzt von ist blieb, glück deinen muß da mir's, nicht glaube zurück träume o ort und. Schnelle zurück einz'ges glaube du dame darfst in, ist gartens vom ort nicht. Der zürntest komm und vaterland zurück wo weh deinen. Ankleiden manchmal ich denkst denkst kleinem stund' denkst, doch im zürnen du es, ja vögel.
    </div>
</body>
</html>
```

<br>

## Chapter 12

### CSS Color Keywords

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Color Keywords</title>
    <style>
        body{
            color: dodgerblue;
        }
        div{
            box-shadow: 0px 0px 15px currentcolor;
            border: 5px solid currentcolor;
            padding: 15px;
        }
    </style>
</head>
<body>
    <h2>The currentcolor Keyword</h2>
    <p>This is some text in the body part...</p>
    <div>
        <p>This div's border color and shadow color is set to the current color value of the body element.</p>
    </div>
</body>
</html>
```

<br>

## Chapter 13

### CSS Combinators

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Combinators</title>
    <style>
        /* Descendant Selector */
        #div1 p{background-color: tomato;}

        /* Child Selector */
        div > p{background-color: lightskyblue;}
    </style>
</head>
<body>
    <!-- Descendant Selector -->
    <h1>Descendant Selector</h1>
    <p>The descendant selector matches all elements that are descendants of a specified element. The following example selects all p elements inside div elements:</p>
    <div id="div1">
        <p>Paragraph 1 in the div.</p>
        <p>Paragraph 2 in the div.</p>
        <p>Paragraph 3 in the div.</p>
    </div>
    <p>Paragraph 4 Not in a div.</p>
    <p>Paragraph 5 Not in a div.</p>

    <!-- Child Selector -->
    <h1>Child Selector (>)</h1>
    <p>The child selector selects all elements that are the children of a specified element. The following example selects all p elements that are children of a div element:</p>
    <div>
        <p>Paragraph 1 in the div.</p>
        <p>Paragraph 2 in the div.</p>
        <section>
            <p>Paragraph 3 in the div (inside a section element).</p>
        </section>
        <p>Paragraph 4 in the div.</p>
    </div>
    <P>Paragraph 5 Not in a div.</P>
    <P>Paragraph 6 Not in a div.</P>


    <!-- Adjacent Sibling Selector -->
    <h1>Adjacent Sibling Selector (+)</h1>
    <p>The adjacent sibling selector is used to select an element that is directly after another specific element.</p>
    <!-- Example div + p {background-color: red;} -->


    <!-- General Sibling Selector -->
    <h1>General Sibling Selector (~)</h1>
    <p>The general sibling selector selects all elements that are next siblings of a specified element.</p>
    <!-- Example div ~ p {background-color: red;} -->
</body>
</html>
```

<br>

## Chapter 14

### CSS Counters

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Counters</title>
    <style>
        body{
            counter-reset: section;
        }
        h1{
            counter-reset: subsection;
        }
        h1::before{
            counter-increment: section;
            content: "Section " counter(section) ". ";
        }
        h2::before{
            counter-increment: subsection;
            content: counter(section) "." counter(subsection) " ";
        }
    </style>
</head>
<body>
    <h1>HTML Tutorial</h1>
    <h2>HTML</h2>
    <h2>CSS</h2>
    <h2>JavaScript</h2>

    <h1>CSS Tutorial</h1>
    <h2>HTML</h2>
    <h2>CSS</h2>
    <h2>JavaScript</h2>

    <h1>JS Tutorial</h1>
    <h2>HTML</h2>
    <h2>CSS</h2>
    <h2>JavaScript</h2>
</body>
</html>
```

<br>

## Chapter 15

### CSS Overflow

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Layout - Overflow</title>
    <style>
        #overflow-test{
            background-color: lightsalmon;
            color: black;
            padding: 15px;
            width: 25%;
            height: 100px;
            border: 1px solid tomato;
            overflow: scroll;
        }
    </style>
</head>
<body>
    <div id="overflow-test">Mit um die euren vor tönen freundschaft klage gut, steigen lied lispelnd nun alten gut. Ihr herzen ersten blick freundliche unbekannten. Wieder gedränge alten gedränge stunden ich ihr mild. Gedränge ersten und naht entwöhntes mich, froher bringt der welt strenge froher mir wahn labyrinthisch wohl, macht irren ich halbverklungnen sie irren es hören wird noch. Gleich schmerz halbverklungnen erfreuet herz euch mein mich faßt, ihr zauberhauch und wohl ich sich, tränen erste sie naht hören zug, sich wiederholt vom lied und mit zu mein stillen beifall, die der gleich ich gedränge sich lebens gestalten, zu halbverklungnen wie diesmal aus guten.</div>
</body>
</html>
```

<br>

## Chapter 16

### CSS Media Queries

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Media Queries</title>
    <style>
        body{
            background-color: tan;
            color: black;
        }

        @media screen and (max-width: 992px){
            body{
                background-color: blue;
                color: white;
            }
        }
        @media screen and (max-width: 600px){
            body{
                background-color: olive;
                color: white;
            }
        }
    </style>
</head>
<body>
    <h1>Resize the browser window to see the effect!</h1>
    <p>By default, the background color of the document is "tan". If the screen size is 992px or less, the color will change to "blue". If it is 600px or less, it will change to "olive".</p>
</body>
</html>
```

<br>

## Chapter 17

### CSS Gradients

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Gradients</title>
    <style>
        .css1{
            background-image: linear-gradient(to right,Tomato,DodgerBlue,MediumSeaGreen,SlateBlue,Violet,LightGray,Orange);
            width: 500px;
            height: 300px;
        }
        .css2{
            background-image: linear-gradient(to bottom right,Tomato,DodgerBlue,MediumSeaGreen,SlateBlue,Violet,LightGray,Orange);
            width: 500px;
            height: 300px;
        }
        .css3{
            background-image: linear-gradient(180deg,Tomato,DodgerBlue,MediumSeaGreen,SlateBlue,Violet,LightGray,Orange);
            width: 500px;
            height: 300px;
        }
        .css4{
            background-image: radial-gradient(circle,SlateBlue,MediumSeaGreen,DodgerBlue,Tomato,Violet,LightGray,Orange);
            width: 500px;
            height: 500px;
        }
        .css5{
            background-image: conic-gradient(DodgerBlue,Tomato,Violet,MediumSeaGreen);
            border-radius: 50%;
            width: 500px;
            height: 500px;
        }
    </style>
</head>
<body>
    <div class="css1">
        <h1></h1>
    </div>

    <div class="css2">
        <h1></h1>
    </div>

    <div class="css3">
        <h1></h1>
    </div>

    <div class="css4">
        <h1></h1>
    </div>

    <div class="css5">
        <h1></h1>
    </div>
</body>
</html>
```

<br>

## Chapter 18

### CSS Pagination

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Pagination Examples</title>
    <style>
        .center{
            text-align: center;
        }
        .pagination{
            display: inline-block;
        }
        .pagination a{
            color: black;
            float: left;
            padding: 8px 16px;
            text-decoration: none;
            transition: background-color .3s;
            border-radius: 5px;
            font-size: 25px;
            /* border: 1px solid #ddd; */
            /* margin: 0 4px; */
        }
        .pagination a.active{
            background-color: #4CAF50;
            color: white;
            border-radius: 5px;
            /* border: 1px solid #4CAF50; */
        }
        .pagination a:hover:not(.active) {
            background-color: #ddd;
        }
    </style>
</head>
<body>
    <div class="center">
        <div class="pagination">
            <a href="#">&laquo;</a>
            <a href="#">1</a>
            <a href="#" class="active">2</a>
            <a href="#">3</a>
            <a href="#">4</a>
            <a href="#">5</a>
            <a href="#">6</a>
            <a href="#">&raquo;</a>
        </div>
    </div>
</body>
</html>
```

<br>

## Chapter 19

### CSS Transforms

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Transforms</title>
    <style>
        #div1{
            width: 200px;
            height: 200px;
            background-color: dodgerblue;
            text-align: center;
            margin: 0 auto;
            margin-top: 200px;
            transition: 2s;
        }
        #div1:hover{
            transform: scale(3) rotate(360deg);
            /*
            transform: skew(-45deg);
            transform: translate(150px, 250px);
            */
        }
    </style>
</head>
<body>
    <div id="div1">
        <h1>Destruction</h1>
    </div>
</body>
</html>
```

<br>

## Chapter 20

### CSS Animations

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Animations</title>
    <style>
        div{
            width: 100px;
            height: 100px;
            position: relative;
            background-color: tomato;
            animation-name: demo;
            animation-duration: 4s;
            animation-delay: 2s;
            animation-iteration-count: 2;
            animation-direction: normal;
        }
        @keyframes demo{
            0%{
                background-color: tomato;
                left: 0px;
                top: 0px;
            }
            25%{
                background-color: dodgerblue;
                left: 200px;
                top: 0px;
            }
            50%{
                background-color: mediumseagreen;
                left: 200px;
                top: 200px;
            }
            75%{
                background-color: violet;
                left: 0px;
                top: 200px;
            }
            100%{
                background-color: #2400a5;
                left: 0px;
                top: 0px;
            }
        }

        /*
        #div1{
            animation-timing-function: linear;
        }
        #div2{
            animation-timing-function: ease;
        }
        #div3{
            animation-timing-function: ease-in;
        }
        #div4{
            animation-timing-function: ease-out;
        }
        #div5{
            animation-timing-function: ease-in-out;
        }
        */
    </style>
</head>
<body>
    <div></div>
</body>
</html>
```

<br>

## Chapter 21

### CSS Lists

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Lists</title>
    <style>
        ol{
            list-style-type: upper-roman;
            list-style-image: url();
            list-style-position: outside;

            background-color: #ff9999;
            padding: 20px;
        }
        ol li{
            background-color: #ffe5e5;
            color: darkred;
            padding: 5px;
            margin-left: 35px;
        }
        ul{
            background-color: #3399ff;
            padding: 20px;
        }
        ul li{
            background-color: #cce5ff;
            color: darkblue;
            margin: 5px;
            padding: 5px;
        }
    </style>
</head>
<body>
    <h1>Styling Lists With Colors</h1>

    <ol>
        <li>HTML</li>
        <li>CSS</li>
        <li>JS</li>
    </ol>
    <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JS</li>
    </ul>
</body>
</html>
```

<br>

## Chapter 22

### CSS Layout - The Display Property

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Layout - The Display Property</title>
    <style>
        li {display: inline;}
        span {display: block;}
        h2.hidden {display: none;}
        h3.hide {visibility: hidden;}
    </style>
</head>
<body>
    <h1>Display a list of links as a horizontal menu:</h1>
    <ul>
        <li><a href="https://youtube.com/">⌨Youtube</a></li>
        <li><a href="https://youtube.com/">⌨Facebook</a></li>
        <li><a href="https://youtube.com/">⌨Twitter</a></li>
    </ul>

    <span>A display property with</span> <span>a value of "block" results in</span> <span>a line break between each span elements.</span>
    <h1>This is a visible heading</h1>
    <h2 class="hidden">This is a hidden heading</h2>
    <h1>This is a visible heading</h1>
    <h3 class="hide">This is a hidden heading</h3>
    <p>Notice that the hidden heading still takes up space.</p>
</body>
</html>
```

<br>

## Chapter 23

### CSS Layout - The Position Property

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Layout - The Position Property</title>
    <style>
        /* Static Position */
        div.static{
            position: static;
            border: 2px dashed teal;
        }


        /* Relative Position */
        div.relative{
            position: relative;
            border: 2px dashed dodgerblue;
            left: 50px;
            width: 50%;
        }


        /* Fixed Position */
        div.fixed{
            position: fixed;
            border: 2px dashed tomato;
            width: 250px;
            right: 0;
            bottom: 0;
        }


        /* Absolute Position */
        div.relat{
            position: relative;
            border: 2px solid lightseagreen;
            width: 400px;
            height: 200px;
        }
        div.absolute{
            position: absolute;
            border: 2px solid lightskyblue;
            width: 200px;
            height: 100px;
            top: 80px;
            right: 0;
        }


        /* Sticky Position */
        div.sticky{
            position: -webkit-sticky;
            position: sticky;
            border: 2px solid MediumSeaGreen;
            padding: 5px;
            top: 0;
            background-color: lightgreen;
        }
    </style>
</head>
<body>
    <!-- Static Position -->
    <h1>position:static</h1>
    <p>HTML elements are positioned static by default. Static positioned elements are not affected by the top, bottom, left, and right properties. An element with static-position is not positioned in any special way; it is always positioned according to the normal flow of the page:</p>
    <div class="static">This div element has position-static</div> <br>


    <!-- Relative Position -->
    <h1>position:relative</h1>
    <p>An element with position-relative is positioned relative to its normal position. Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position. Other content will not be adjusted to fit into any gap left by the element.</p>
    <div class="relative">This div element has position-relative</div> <br>


    <!-- Fixed Position -->
    <h1>position:fixed</h1>
    <p>An element with position-fixed is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element. A fixed element does not leave a gap in the page where it would normally have been located.</p>
    <div class="fixed">This div element has position-fixed</div> <br>


    <!-- Absolute Position -->
    <h1>position:absolute</h1>
    <p>An element with position-absolute is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed). However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling. Note: Absolute positioned elements are removed from the normal flow, and can overlap elements.</p>
    <div class="relat">This div element has position-relative
        <div class="absolute">This div element has position-absolute</div>
    </div> <br>


    <!-- Sticky Position -->
    <h1>position:sticky</h1>
    <p>An element with position-sticky is positioned based on the user's scroll position. A sticky element toggles between relative and fixed, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place (like position:fixed).</p>
    <div class="sticky">I am sticky!</div>
    <div style="padding-bottom: 2000px;">
        <p>S lovak ott hoz kettős ha ahol miatt énekem. Elevenek vakogjatok de szenvedi hű minden végett. Ruha élő is öl igát így fáj a a, hozzám laktok végző ha az..</p>
        <p>Alegrísima arcos es los de paso de loca ojos, golondrina vuelve de repartiendo deja la, al borrachos hule arcos con y hule el sillas. Se y el manteles con los.</p>
        <p>Brust lachtet die so hab ich du wo du zürntest. Gehofft du muß du liebe der dir mir's. Teuren geschaut ward wo liebe die träume einz'ges sanftes nicht, du teuren.</p>
    </div>

    <!-- Top-Left-Position{top: 8px; left: 16px;} Top-Right-Position{top: 8px; right: 16px;} -->
    <!-- Centered-Position {text-align: center; top: 50%; width: 100%;} -->
    <!-- Bottom-Left-Position{bottom: 8px; left: 16px;} Bottom-Right-Position{bottom: 8px; right: 16px;} -->
</body>
</html>
```

<br>

## Chapter 24

### CSS Buttons

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Buttons</title>
    <style>
        a:link, a:visited{
            color: white;
            background-color: #f35045;
            text-decoration: none;
            padding: 15px 25px;
            text-align: center;
            display: inline-block;
        }
        a:hover{
            color: #03d4d4;
            background-color: black;
            font-family: Verdana, Geneva, Tahoma, sans-serif;
        }
        a:active{
            color: black;
            background-color: #03d4d4;
        }
    </style>
</head>
<body>
    <a href="https://youtube.com/" target="_blank">YouTube</a>
</body>
</html>
```

<br>

## Chapter 25

### CSS Tooltip

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Tooltip</title>
    <style>
        body{
            text-align: center;
        }

        .tooltip{
            position: relative;
            display: inline-block;
            border-bottom: 1px dashed black;
        }

        .tooltip .tooltiptext1{
            visibility: hidden;
            width: 120px;
            background-color: black;
            color: #fff;
            text-align: center;
            border-radius: 6px;
            padding: 5px 0;

            /* Position the tooltiptext */
            position: absolute;
            z-index: 1;
            top: -5px;
            left: 110%;

            opacity: 0;
            transition: opacity 1s;
        }
        /* Arrow Added */
        .tooltip .tooltiptext1::after{
            content: "";
            position: absolute;
            top: 50%;
            right: 100%;
            margin-top: -5px;
            border-width: 5px;
            border-style: solid;
            border-color: transparent black transparent transparent;
        }

        .tooltip .tooltiptext2{
            visibility: hidden;
            width: 120px;
            background-color: black;
            color: #fff;
            text-align: center;
            border-radius: 6px;
            padding: 5px 0;

            /* Position the tooltiptext2 */
            position: absolute;
            z-index: 1;
            top: -5px;
            right: 110%;

            opacity: 0;
            transition: opacity 1s;
        }
        /* Arrow Added */
        .tooltip .tooltiptext2::after{
            content: "";
            position: absolute;
            top: 50%;
            left: 100%;
            margin-top: -5px;
            border-width: 5px;
            border-style: solid;
            border-color: transparent transparent transparent black;
        }

        .tooltip .tooltiptext3{
            visibility: hidden;
            width: 120px;
            background-color: black;
            color: #fff;
            text-align: center;
            border-radius: 6px;
            padding: 5px 0;

            /* Position the tooltiptext3 */
            position: absolute;
            z-index: 1;
            bottom: 150%;
            left: 50%;
            margin-left: -60px;

            opacity: 0;
            transition: opacity 1s;
        }
        /* Arrow Added */
        .tooltip .tooltiptext3::after{
            content: "";
            position: absolute;
            top: 100%;
            left: 50%;
            margin-left: -5px;
            border-width: 5px;
            border-style: solid;
            border-color: black transparent transparent transparent;
        }

        .tooltip .tooltiptext4{
            visibility: hidden;
            width: 120px;
            background-color: black;
            color: #fff;
            text-align: center;
            border-radius: 6px;
            padding: 5px 0;

            /* Position the tooltiptext4 */
            position: absolute;
            z-index: 1;
            top: 150%;
            left: 50%;
            margin-left: -60px;

            opacity: 0;
            transition: opacity 1s;
        }
        /* Arrow Added */
        .tooltip .tooltiptext4::after{
            content: "";
            position: absolute;
            bottom: 100%;
            left: 50%;
            margin-left: -5px;
            border-width: 5px;
            border-style: solid;
            border-color: transparent transparent black transparent;
        }

        .tooltip:hover .tooltiptext1{
            visibility: visible;
            opacity: 1;
        }
        .tooltip:hover .tooltiptext2{
            visibility: visible;
            opacity: 1;
        }
        .tooltip:hover .tooltiptext3{
            visibility: visible;
            opacity: 1;
        }
        .tooltip:hover .tooltiptext4{
            visibility: visible;
            opacity: 1;
        }
    </style>
</head>
<body>
    <h2>Move the mouse over the text below:</h2><br>

    <div class="tooltip">Hover over me
        <span class="tooltiptext1">Tooltip text</span>
        <span class="tooltiptext2">Tooltip text</span>
        <span class="tooltiptext3">Tooltip text</span>
        <span class="tooltiptext4">Tooltip text</span>
    </div>
</body>
</html>
```

<br>

## Chapter 26

### CSS Transitions Part 1

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Transitions Part 1</title>
    <style>
        .main{
            width: 300px;
            height: 300px;
            background-color: tomato;
            text-align: center;
            margin: 0 auto;
            transition: width 2s, transform 2s;
        }
        h1{
            font-size: 2.5rem;
            color: white;
        }
        .main:hover{
            width: 400px;
            transform: rotate(360deg);
        }
    </style>
</head>
<body>
    <div class="main">
        <h1>Bangladesh</h1>
    </div>
</body>
</html>
```

<br>

## Chapter 27

### CSS Transitions Part 2

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Transitions Part 2</title>
    <style>
        .main{
            background-color: dodgerblue;
            width: 500px;
            height: 300px;
            margin: 0 auto;
            text-align: center;
        }
        h1{
            font-size: 2.5rem;
            color: white;
            transition: font-size 2s;
        }
        h1:hover{
            font-size: 3rem;
        }
    </style>
</head>
<body>
    <div class="main">
        <h1>Bangladesh</h1>
    </div>
</body>
</html>
```

<br>

## Chapter 28

### CSS Transitions Part 3

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Transitions Part 3</title>
    <style>
        .main{
            background-color: mediumseagreen;
            width: 300px;
            height: 300px;
            margin: 0 auto;
            transition-property: width;
            transition-duration: 1s;
            transition-timing-function: linear;
        }
        .main:hover{
            width: 400px;
        }
    </style>
</head>
<body>
    <div class="main">
        <h1>Bangladesh</h1>
    </div>
</body>
</html>
```

<br>

## Chapter 29

### CSS Tables

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Tables</title>
    <style>
        /* Table No 1 */
        #customers{
            width: 100%;
            border-collapse: collapse;
            font-family: Arial, Helvetica, sans-serif;
        }
        #customers th, #customers td{
            border: 2px solid #ddd;
            padding: 10px;
        }
        #customers tr:nth-child(even){
            background-color: #f2f2f2;
        }
        #customers tr:hover{
            background-color: #ddd;
        }
        #customers th{
            color: white;
            background-color: #04AA6D;
            text-align: left;
            padding-top: 12px;
            padding-bottom: 12px;
        }

        /* Table No 2 */
        #table2{
            width: 100%;
            border: 1px dashed black;
            border-collapse: collapse;
        }
        #table2 th, #table2 td{
            text-align: left;
            padding: 10px;
        }
        #table2 tr:nth-child(even){
            background-color: #f2f2f2;
        }
    </style>
</head>
<body>
    <!-- Table No 1 -->
    <table id="customers">
        <thead>
            <tr>
                <th>Company</th>
                <th>Contact</th>
                <th>Country</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Alfreds Futterkiste</td>
                <td>Maria Anders</td>
                <td>Germany</td>
            </tr>
            <tr>
                <td>Berglunds snabbköp</td>
                <td>Christina Berglund</td>
                <td>Sweden</td>
            </tr>
            <tr>
                <td>Centro comercial Moctezuma</td>
                <td>Francisco Chang</td>
                <td>Mexico</td>
            </tr>
            <tr>
                <td>Königlich Essen</td>
                <td>Philip Cramer</td>
                <td>Germany</td>
            </tr>
            <tr>
                <td>Ernst Handel</td>
                <td>Roland Mendel</td>
                <td>Austria</td>
            </tr>
        </tbody>
    </table>

    <br><br>

    <!-- Table No 2 -->
    <div style="overflow-x: auto;">
    <table id="table2">
        <tr>
            <th>First Name</th>
            <th>Last Name</th>
            <th>Points</th>
            <th>Points</th>
            <th>Points</th>
            <th>Points</th>
            <th>Points</th>
            <th>Points</th>
            <th>Points</th>
            <th>Points</th>
            <th>Points</th>
            <th>Points</th>
        </tr>
        <tr>
            <td>Toufiq</td>
            <td>Gilani</td>
            <td>50</td>
            <td>50</td>
            <td>50</td>
            <td>50</td>
            <td>50</td>
            <td>50</td>
            <td>50</td>
            <td>50</td>
            <td>50</td>
            <td>50</td>
        </tr>
        <tr>
            <td>Rus</td>
            <td>Putin</td>
            <td>80</td>
            <td>80</td>
            <td>80</td>
            <td>80</td>
            <td>80</td>
            <td>80</td>
            <td>80</td>
            <td>80</td>
            <td>80</td>
            <td>80</td>
        </tr>
        <tr>
            <td>Turk</td>
            <td>Erdogan</td>
            <td>75</td>
            <td>75</td>
            <td>75</td>
            <td>75</td>
            <td>75</td>
            <td>75</td>
            <td>75</td>
            <td>75</td>
            <td>75</td>
            <td>75</td>
        </tr>
    </table>
    </div>
</body>
</html>
```

<br>

## Chapter 30

### CSS Specificity

#### What is Specificity?

- If there are two or more CSS rules that point to the same element, the selector with the highest specificity value will "win", and its style declaration will be applied to that HTML element.

#### How to Calculate Specificity?

![CSS Specificity](https://user-images.githubusercontent.com/113186897/203640523-103dbce0-1c39-4ef4-bdad-06efdd747266.png)

<br>

# CSS-TUTORIAL
