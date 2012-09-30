---

title: A Friendly Guide to HTML
layout: default
categories: tutorials

---

## Super Basic Tags

| HTML Tag 	| Purpose 	|
| ---	| ---- 	|
| `<strong> </strong>`	| Makes text bold. (You could use `<b></b>`, but cool people don't.)	|
| `<em></em>`	| Makes text italicized. (`<i></i>` works too, but it's being phased out—don't use it.)	|
| `<h1></h1>`	| Makes a Level 1 Header. 	|
| `<h2></h2>`	| Makes a slightly smaller Level 2 Header. (This goes all the way to `<h6>`, but I'll spare you.) 	|
| `<ul></ul>`	| Makes an unordered list. (Also affectionately known as bullet points.) 	|
| `<ol></ol>`	| Makes an ordered list. (Better known as a numbered list.)	|
| `<p></p>` 	| Makes a paragraph.	|
| `<div></div>`	| One of the most used tags in HTML. It does almost nothing.	|
| `<span></span>` 	| Another useful tag that does absolutely nothing. (We'll get to using these two later.)	|

There are many more tags, but these should get you off the ground. If you find yourself needing to make table of information, we can talk about HTML's myriad of tags associated with making table. Same thing for forms. It's a lot to swallow at first, but it's not that hard once you get the hang of it. **Just remember**: You have to close (almost) every tag you open or there will be tears.

## Setting Attributes and Gluing the Web Together

With the basic tags above, you'll be able to create a basic web page. That's great and wonderful. If you've used the web for more than about five seconds, you'll realize that were missing two things—links and images.

* Links get you from one page to another.
* Images are pretty.

I skipped them for one reason: We didn't talk about attributes yet. Attributes are easy. Basically, they are extra information that you include in a tag to make things a little more awesome.

Here is a fake example:

	<tag attribute="pineapple">Some Text</tag>

Things to notice:

1. The attribute only goes in the opening tag. You don't need to include it in the ending tag.
2. The extra information (`pineapple` in this case) goes in double-quotes.
3. There is no three.

### Making Links ###

Links hold the web together. So, let's make some links.

Let's say you want to link to [Google][]. (Who doesn't want to link to Google?) You'd write a tag that looks a lot like this:

[Google]: http://google.com/

	<a href="http://google.com">This is a link to Google</a>

There are some weird words in here. I'll explain:

* For some reason, the tag we use for links is the `<a></a>` tag—which has something to do with an anchor.
* The `href` attribute sets the destination of the link.. In this case, our link points to `http://google.com`. There are other attributes that are commonly used, but I've left them out for clarity.
* Whatever words you want to be used in the link appears between the tags.

### Inserting Images ###

You can include images in your pages. These images are either in the same folder as your HTML (or a sub-folder nearby) or hosted on somebody else site. Including images stored on someone else's server is a recipe for bad news and typically considered to be poor sportsmanship.[^1] That's not going to stop us as we're learning the ropes, but it's not something you should be doing once we remove the training wheels off your bike.

Put on your imagination caps for a moment, please:

* Let's say I wanted to include an image of a taco in my web page.
* Let's also say that my picture was stored in a file named `taco.jpg` and it was in the same folder as my HTML file.
* Finally, let's assume I was going to have tacos for lunch. This has little to nothing to do with this example, but it makes me happy and I prefer to be happy whenever the opportunity arises.

Here is how I would include my taco image:

	<img src="taco.jpg">

Okay, I have an `<img>` tag. That's good. In that tag I have an attribute called `src` which points to the source of my image. Great.

**WAIT—WHOA—WHAT!?!** You may be asking, "Where is the closing tag? You told me I always had to have a closing tag. Why did you lie to me? Do you hate me?" (If you're not asking those questions right now, you probably haven't been paying attention. Stop playing around on the computer and listen to me.)

The `<img>` doesn't have a closing tag. Deal with it. The `<img>` tag is one of those tags that lives alone and buys a suspicious amount of cat food from Key Food when it goes on sale. There is a story behind this, if you really want to know, then ask me later.

[^1]: If you pull in images from someone else's server, you're making their server do more work and slowing down their site by taking up their bandwidth. People tend not to like this. Also, if you link to a image on my server and I move or delete the image, then it will most likely break your site. Moral: host your own images.
