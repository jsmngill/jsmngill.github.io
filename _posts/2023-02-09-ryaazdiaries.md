## Another Day Another Concepts!

***“Programming isn’t about what you know; it’s about what you can figure out.”
– Chris Pine***

Back Again! 
As I have shared the website in the previous blog my mentor reviewed it and suggested me change some things in it. I was working on that for the last two days, and still on it as I had to pause the challenge because my mentor suggested me to study the concepts of combinators and grouping selectors as he felt the need for me to understand the concepts, after reviewing my code. So here is what I understood about the aforementioned topics.

1.**Combinators**: This is the property that explains the relationship between the selectors. There are four types of combinators:

1.1 **Descendant Combinator**: Denoted by blank-space(“ ”). It combines two selectors such that the elements matched by the second selector are selected only if they have an ancestor element matching the first selector.
**Example**: HTML code:
```
<div class= “box” <p> Hello </p> </div>
	      <p> Hi </p>
```        
CSS code:
```
.box p{
Color: red;
}
```
**Output**:
“Hello” will be printed in red color.
    	
1.2. **Child Combinator**: it is depicted by (>), and is placed between two selectors. 
It matches only those elements matched by the second selector that is the 
direct children of elements matched by the first.

**Example**: HTML code:
```
<ul>
    <li>Unordered item</li>
    <li>Unordered item
        <ol>
            <li>Item 1</li>
            <li>Item 2</li>
        </ol>
    </li>
</ul>
```
CSS code:
```
ul > li {
    border-top: 5px solid red;
} 
```
**Output**: The first “Unordered item” will have the border top.

1.3. **Adjacent Sibling Combinator**: It is symbolized by (+), and is placed between
 two CSS selectors. It matches only those elements matched by the second 
selector which is the next sibling element of the first selector.

**Example**: HTML:
```
<article>
    <h1>GitHub</h1>
    <p>Veggies es bonus vobis, proinde vos postulo essum magis kohlrabi 
         welsh onion daikon amaranth tatsoi tomatillo melon azuki bean garlic.</p>

    <p>Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot 
           courgette tatsoi pea sprouts fava bean collard</p>
</article>
```
**Output**: paragraph 1 would have the properties of the CSS.

1.4. **General Sibling Combinator**: It is denoted by **(~)** and is used to select the siblings that are not directly adjacent.

**Example**:
```
p~img
```
(it is used to select all img elements, that comes anywhere after paragraph tag)

2. **Grouping Selector**: CSS selectors that exclusively apply styles to a single element, a class, an ID, or both. However, CSS also makes it relatively simple to target several elements at once in order to support particular CSS properties and rules. To do this, separate the names of the selectors with a comma, and you are ready to apply CSS styles to a variety of items.
**Example**: 
```
h1, h2{
     	font-family: Verdana, sans-serif;
}
```

This was my learning for two days, will be sharing the more of my daily professional diary!

Will see you soon!

~J Gill







