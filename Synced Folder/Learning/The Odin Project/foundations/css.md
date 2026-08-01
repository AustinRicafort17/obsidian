#TOP #Learning 
is the language that goes on top of an html file that give a website *style*

![[css.jpg]]

selectors
-is the "target" of the styling 
	the universal selector is * (asterisk)

type selectors
-targets a type of elements like <div> <p> or <h1>

class selectors 
-targets a class of elements. 
	if i had given multiple elements the class "dog"
	i would give all "dog" elements blue text by doing:
	.dog {
		color: blue; }
	there must be . before the selector

id selectors
-targets an id of elements
	mostly used for specific elements and has high priority in css.
	if there was an element with both an id and a class, any id selectors property would go over the class selectors property.
	 if in a class of blue dogs id like to give this one particular dog, for some odd reason, yellow text.
	i would go :
```
		#dog {
			color: yellow ;}
```
	there must be a "#" in the start of the selector


I can group selectors together so they can share similar properties but also have separate selectors of their own

```.dogs,
.cats{
	height: 200px;
}
```
.dogs {
	color:blue;
}
.cats{
	color:red;
}


i can chain selectors so that i can target a specific element 

.dogs.puppy {
	color: green;
}

.dog#corgi {
	color: orange;
	}
	
it finds the element with these properties



descendant combinators
- make it so i can target a specific element depending on its nesting. separate the selectors with a space.

.dog .puppy {
	color: green
}
