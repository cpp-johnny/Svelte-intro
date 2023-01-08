
<!--- start --->
<script>
	let src = '/image.gif';
</script>

<img />

<!---
Just like you can use curly braces to control text, 
you can use them to control element attributes.

Our image is missing a src — let's add one:
--->
<script>
	let src = '/image.gif';
</script>

<img />

<img src={src}/>

<!---

That's better. But Svelte is giving us a warning:

A11y: <img> element should have an alt attribute

When building web apps, it's important to make sure that they're accessible to the broadest possible userbase, including people with (for example) impaired vision or motion, or people without powerful hardware or good internet connections. Accessibility (shortened to a11y) isn't always easy to get right, but Svelte will help by warning you if you write inaccessible markup.

In this case, we're missing the alt attribute that describes the image for people using screenreaders, or people with slow or flaky internet connections that can't download the image. Let's add one:


We can use curly braces inside attributes. Try changing it to "{name} dances." — remember to declare a name variable in the <script> block.


--->

<!--- solution --->
<script>
	let src = '/image.gif';
	let name = 'Rick Astley';
</script>

<img {src} alt="{name} dances." />
