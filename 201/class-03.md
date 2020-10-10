## Class 3
# Section 1: HTML & CSS
# Listes 
## 1. Lists Types
### HTML provides us with three different types:
- Ordered list <'ol'>
- Unordered list <'ul'>
- Definition list <'dl'>
* Each item in the list is placed between an opening <'li'> tag and a closing </'li'> tag. (The li stands for list item.)

#### The definition list is created with the <'dl'> element and usually consists of a series of terms and their definitions.
#### Inside the <'dl'> element you will usually see pairs of <dt> and <'dd'> elements.

## 2. Nested lists 
#### You can put a second list inside an <'li'> element to create a sublist or nested list. Browsers display nested lists indented further than the parent list. In nested unordered lists, the browser will usually change the style of the bullet point too.

# Boxes in CSS 
#### CSS treats each HTML element as if it lives in its own box.

## 1. Box dimentions
#### you can control the dimentions by hieght and width property, see the following example:
> div.box {
  height: 300px;
  width: 300px;
  background-color: #bbbbaa;}

## 2. Limiting width
#### you can **LIMITING THE WIDTH** to expand and shrink to fit the size of the user's screen, so the min-width property specifies the smallest size a box can be displayed at when the browser window is narrow, and the max-width property indicates the maximum width a box can stretch to when the browser window is wide. see this example:

>td.description {
 min-width: 450px;
 max-width: 650px;
 text-align: left;
 padding: 5px;
 margin: 0px;}

## 3. Limiting height
#### And for sure you can **LIMIT THE HIEGHT** eather by [min-height, max-height], see the following examples:
> p {
 min-height: 10px;
 max-height: 30px;}

## 4. Overflowing Content
#### The overflow property tells thebrowser what to do if the contentcontained within a box is largerthan the box itself. It can haveone of two values:
- `hidden` This property simply hides anyextra content that does not fit inthe box.
- `scroll` This property adds a scrollbar tothe box so that users can scrollto see the missing content.
> p.one {
 overflow: hidden;}
 p.two {
 overflow: scroll;}


# Border, Margin & Padding
#### Every box has three available properties that can be adjusted to control its appearance.
#### The padding and margin properties are very helpful in adding space between various items on the page.


#### you can control the border width by this properties , see the following example:
> p.one {
> border-width: 2px;}
> p.two {
> border-width: thick;}
> p.three {
> border-width: 1px 4px 12px 4px;}
#### Or you can control the sides separetly by these: 
> border-top-width
> border-right-width
> border-bottom-width
> border-left-width

 #### You can control the style of a border using the border-style property. This property can take the following values:
 > p.one {border-style: solid;}
 > p.two {border-style: dotted;}
 > p.three {border-style: dashed;}
 > p.four {border-style: double;}
 > p.five {border-style: groove;}
 > p.six {border-style: ridge;}
 > p.seven {border-style: inset;}
 > p.eight {border-style: outset;}

#### You can specify the color of a border using either RGB values, hex codes or CSS color names 
> p.one {
> border-color: #0088dd;}
Or 
> border-top-color
> border-right-color
> border-bottom-color
> border-left-color

## Shorthand 
#### The border property allows you to specify the width, style and color of a border in one property (and the values should be coded in that specific order). like this: 
> p {
> width: 250px;
> border: 3px dotted #0088dd;}

# display proparity 
#### The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page. The values this property can take are:
- inline
- block
- inline-block
- none

> Block-level boxes can be made into inline boxes, and inline boxes made into block-level boxes.
> Legibility can be improved by controlling the width of boxes containing text and the leading.
> CSS3 has introduced the ability to create image borders and rounded borders.



# Dicision & Loops

- There are two component to dicision:
  1. expression returns value
  2. condition says what to do in givin satuation

#### At the most basic level, you can evaluate two variables using a comparison operator to return a t rue or f al se value. see the nex ex.
> var pass = 50; II Pass mark
> var score = 90; II Score
> II Check if t he user has passed
> var hasPassed = score >= pass;
> II Write the message i nt o the page
> var el = document .getEl ementByld(' answe r ');
> e 1 . t extContent = 'Leve 1 passed: ' + has Passed; 

#### the operation normally we use with loop as follow:

> Not A,!A
> And ,&&
> OR,"||"
> greater than,">"
> Less than,"<"

## USING IF ... ELSE TATEMENTS
#### f ... e 1 se statement allows you to provide two sets of code:
1. one set if the condition evaluates to true
2. another set if the condition is false 

## Switch statment 
#### perform differant actions for differant condition 
###### see the next example:


> switch (level) {
> case 1:
> msg = 'Good luck on the first test ' ;
> break;
> default :
> msg = 'Good l uck!';
> break;
> var el = document.getEl ementByld('answer');
> el .textContent = msg; 


# Loops
### There are three differant type of loops:
## 1. While 
![whileloop](https://www.tutorialspoint.com/javascript/images/while_loop.jpg)
#### the code will contuniue to loop as long sa the condition is true. it used normally when you do not know how many the code will run.
> While (condition){code..;}

## 2. for 
![forloop](https://www.tutorialspoint.com/javascript/images/for_loop.jpg)
#### the code will contuniue to loop as long sa the condition is true. it used normally when you do know how many the code will run.
## 3. Do while
![Dowhile](https://cdn.journaldev.com/wp-content/uploads/2017/10/java-do-while-loop-1.png)
#### similar to while loop but the differance it will always run the statment in side the curly pbraces at least once even the condation false.
