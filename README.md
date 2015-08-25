# mixend

Just a single Sass file containing a list of useful mixins and functions for front-end development. 

## why?

Libs like Bourbon & Compass are awesome but I have found to be a bit overkill. Many mixins are used for vendor prefixing, which are slowly becoming obsolete due to tools like Autoprefixer. In response, my aim is to compile a list of mostly utility & helper mixins and functions that extend beyond Sass's built in functionality. 

## Docs

### Utilities

#### clearfix
A clearfix shorthand.

Usage:
```
.container {
	@include clearfix;
}
```

### Responsive

#### media
A shorthand for quickly writing a media query. Takes a string of 'min' or 'max' for direction, and then a breakpoint.

Usage:
```
.sidebar {
	@include media('min', 768px){
		width: 25%;
	}
}
```

### Helper Functions

### tint
Takes a color and percentage as arguments and makes the color said percentage "whiter"

Usage:
```
h1:hover {
	color: tint(blue, 10%);
}
```

### shade
Takes a color and percentage as arguments and makes the color said percentage "blacker"

Usage:
```
h1:hover {
	color: shade(blue, 20%);
}
```

More to come...