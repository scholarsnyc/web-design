---

title: An Introduction to CSS
layout: default
categories: tutorials

---

When last we spoke, we looked at how to do some basic styling in CSS. It's pretty easy to make all of the `<p>` tags in a page hot pink, but what if you only want a few of the paragraphs to be hot pink? Or, perhaps, let's say that you want to use the same style for a few different tags? How do you do that?
	
It turns out that it's not all that hard to get granular about what you want to style and how you want to style it in CSS. The trick is that you need to add a little bit more information to your HTML markup.

On any tag in HTML, you can set an extra attribute called `class`. Adding a class to an HTML tag is kind of like tagging a friend in a picture on Facebook. You can add as many classes as you want to a given HTML tag.

Here is an example:

	<h1>This is a heading</h1>
	<p>This is a paragraph.</p>
	<p class="special">This is a paragraph with the "special" class applied to it.</p>
	<p class="special secret">This paragraph has two classes applied to it.</p>
	
If you want to use more than one tag, then you need to separate each class with a space. Pretty easy stuff. Adding a class to your HTML is not particularly exciting. You should see no difference from before you added the classes to your markup—unless you messed something up royally, of course.

The magic happens when we define styles for those classes in CSS.

In order to style a class, you need some special syntax. Basically, you prepend the name of your class with a dot.

	.special {
		background-color: yellow;
	}
	
	.secret {
		background-color: white;
		color: white;
	}
	
The dot is important. If you forget to include the dot, your browser will go looking for the `<special>` tag as well as the `<secret>` tag. This is a problem primarily because those two tags don't exist *and* they're not what you wanted.