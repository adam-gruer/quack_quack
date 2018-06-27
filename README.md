# quack_quack
![Count Duckula](img/duckula.png "Picture of count duckula")

## pseudo (quack_quack) code with syntax highlighting from R Markdown and Prism.js

read this blog post from Charles T. Gray http://cantabile.rbind.io/2018/06/26/quack-quack-environment/

## How to use.
Clone or download this project to your machine.

- Edit <code>quack_quack.rmd</code>
- create new code chunks for quack_quack code, insert a new chunk and replace <code>{r}</code> with <code>{quack_quack}</code>
- in quack_quack chunks, the code won't run, this is a GOOD THING. Knitr will warn but will continue processing. 
- any dataset represented like <code>some_dataset</code> and references to <code>quack_quack</code> and <code>column_name</code> will be highlighted in the knitted html output
- regular <code>{r}</code> chunks will be processed.
- save the .rmd and knit to html

## Extending

- more quack_quack keywords can be added by editing <code>scripts/prism.js</code> and adding new tokens with <code>'token_name': regex for keyword(s)</code>
- search for <code>quack_quack</code> in <code>scripts/prism.js</code> to see examples and to be in the correct spot to add new tokens
- to change the css open <code>themes/prism.css</code> and search for <code>.token.quack_quack</code> for an example

View a preview of the knitted htlm file here : https://adam-gruer.github.io/quack_quack/quack_quack.html

The project involves some R Markdown chunk tricks and a customized version of the Prism.js syntax highlighter for R.

**Help wanted** : customizing RStudio syntax highlighting to display the quack_quack syntax natively in .Rmd files in the RStudio editor

