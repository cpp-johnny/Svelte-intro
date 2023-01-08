<!--- new --->

<script>
	let string = `this string contains some <strong>HTML!!!</strong>`;
</script>

<p>{string}</p>


<!---

Ordinarily, strings are inserted as plain text, meaning that characters like < and > have no special meaning.

But sometimes you need to render HTML directly into a component. For example, the words you're reading right now exist in a markdown file that gets included on this page as a blob of HTML.

In Svelte, you do this with the special {@html ...} tag:

--->

<script>
	let string = `this string contains some <strong>HTML!!!</strong>`;
</script>

<p>{@html string}</p>
