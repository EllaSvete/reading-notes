
# What is CSS?

* Stands for Cascading Style Sheets

* Allows you to create the style of a webpage.

* Language that describes how HTML elements look

* CSS is the only way you can visually adjust your website


## CSS Class Notes

- 'Rule': All the CSS styling properties and value that tells and element or a group of elemnents how to look. ex "I wish these words *looked* better
- 'Property': Something that an element uses to describe how it looks
- there is a very big list. You have to loook it up to figure how each property effects our elements. It goes inbetween curly braes or brackets
- 'Value': what you assign to a property. a single string ex. "relative" or "px". The other side of our colon. Sometimes there is more than one value, but you'll have to look up which properties allow multiple values
- 'Selector': Precedes rules of curly braces, is used to select one or more element in the HTML document. for example, instead of 'p' could be something like #intro.
- 'Curly Backets': The rule for our selectors is always within a set of these bracket {}
~
~ 

 '''CSS


 p {
   font-size:10px; - there should always be a pixel value.
   border: 2px dashed black;
   display: relative;
   color: blue;

 }
 '''

 ## Linking CSS:

 < !DOCTYPE html>
< html>
< head>
< link rel="stylesheet" href="mystyle.css">
< /head>
< body>

< h1>This is a heading< /h1>
< p>This is a paragraph.< /p>

</ body>
< /html>

## Color

* Using a color terms that we know: red, blue, aqua, teal, mauve

* RGB: the additive values of red, green, blue.
'color: rgb(255);' - values in the rgb function
rbga - a stands for alpa which is for opactiy, point value to control
* CYMK: The addivitve values of cyan, magenta, yellow, and black - uses percentagess and is subtractive values
* Hex values: a six encoded string made up of the characters of 0-f. Every two characters that respond to ( red/green/blue )
'#000000' - white
'#ffffff' - black
Hex can be a 3 characters like #fff
* HSL stands for Hue Saturation Lightness
example: hsl(0,100%,50%)
can also be hsla

## Moving things

- float: any content that comes after should be on one side or the other side ex float: left;
- Margin: starting from border, move things away from me example 10px. 
- Margin-right: 10px;
- Padding: adding active space, helpful with a border when you don't want content bumping up against the border. Allows negative space inside of an element
- centering: depends on the relationship from parent to children.
  - #heading div {
      width: 150px
      margin: 0 auto
  }
