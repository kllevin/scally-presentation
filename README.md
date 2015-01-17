# Scally CSS framework presentation

A presentation built in: <https://github.com/hakimel/reveal.js> for the
[Scally CSS framework](https://github.com/chris-pearce/scally).

## TODO

- Favicon.
- Create a sub domain for Scally.
- Sync with DB.

## Ideas

### Structure

- How it came about?
- What is it?
	- Lego: bits and pieces to construct UI
	- OOCSS
	-	Responsive ready
	- Sass-based
- What it's not
	- An all singing and all dancing UI component library
	- Examples from Foundation
- Why use it?
	- Why the need?
		-	CSS sucks
		- Anyone can write CSS, writing CSS is easy, architecting it isn’t
		- Everything is in the global scope, it's very leaky!
		- Without a proper architecture/system it’ll turn into a big pile of mud (Show funny pic of Gandolf?)
	- Everything has its place:
		- Gives you an architecture
		- Shouldn’t be left wondering where something lives
	- Unopinionated
	- Everything is configurable
	- Ensures consistency
	- Performant:
		-	Show file size
	- Makes things highly maintainable
	- Rapid UI development
- How to use it
	- Explain each layer (graphic of the 4 layers)
	- Defer more work to the HTML
	- https://github.com/chris-pearce/scally/tree/master/core#settings
	- https://github.com/chris-pearce/scally/tree/master/layout#how-to-use (open up the README to show the screen shots)
	- https://github.com/chris-pearce/scally/tree/master/layout#do-not-mix-other-styles
	- https://github.com/chris-pearce/scally/tree/master/components#how-to-use
	- https://github.com/chris-pearce/scally/tree/master/components#portable-and-robust
	- https://github.com/chris-pearce/scally/tree/master/components#free-of-constraints
	- https://github.com/chris-pearce/scally/tree/master/components#encapsulation
	- https://github.com/chris-pearce/scally/tree/master/utilities#what-are-they
	- https://github.com/chris-pearce/scally/tree/master/utilities#why-have-them
	- https://github.com/chris-pearce/scally/tree/master/utilities#how-to-use
	- https://github.com/chris-pearce/scally/tree/master/utilities#openclose-principle
	- https://github.com/chris-pearce/scally/tree/master/utilities#applying-at-breakpoints
	- Acts as the foundation for all Campaign Monitor UI builds, we than have another layer on top which contains all Campaign Monitor specific styles
	- Setting it up:
		- Bower (more to follow e.g. NPM, Ruby Gem)
		- style.scss
	- Examples (the work horses):
		- Side-by-side
		- List-inline
		- Grid
- How it can help CM
	-	Ensure consistency, look at spacing.
	- Reduce the need for testings.
	- Release features a lot faster.
	- Introduce a CM specific layer on top of Scally, Scally is the scafholding, lick of paint.
- That's a wrap
	- Try it out: `bower install scally`.
	- Some links:
		- This presentation
		- The Scally GH repo (extensive and checkout the **further reading** sections)
		- The WIP Scally website
- Q & A


-------

### Other

- OO programming principles
- Grab all the CodePen code from WF Labs.
- Demo it by showing the CM app built in it
- Show examples of the legacy CSS
- Screen shots of the app and highlight areas where Scally can be used.
- Foundation problems:
	- Too opinionated e.g. table element comes with too many styles: zebra
		strips, cell padding.
- Quotes:
	>> When I start a new project, I assume it will eventually be open sourced (even if it's unlikely). This mindset leads to effortless modularization. If you think about how other people outside your company might use your code, you become much less likely to bake in proprietary configuration details or tightly coupled interfaces. This, in turn, leads to cleaner, more maintainable code. Even internal code should pretend to be open source code.
	http://tom.preston-werner.com/2011/11/22/open-source-everything.html
	>> “Meanwhile, CSS is a simple language. Sass, being intended to write CSS, should not get much more complex than regular CSS. The KISS principle (Keep It Simple Stupid) is key here and may even take precedence over the DRY principle (Don’t Repeat Yourself) in some circumstances.”
	>> CSS had been left to people with a designer’s mind; any code needs the mind of a developer applied to it, someone who gets DRYness, abstraction, efficiency, etc.