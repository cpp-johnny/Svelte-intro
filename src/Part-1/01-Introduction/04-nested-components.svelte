<!--- new in src/app.svelte--->

<p>This is a paragraph.</p>

<style>
	p {
		color: purple;
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}
</style>

<!--- new in src/Nested.svelte --->
<p>This is another paragraph.</p>

<!---

It would be impractical to put your entire app in a single component. Instead, we can import components from other files and include them in our markup.

Add a <script> tag that imports Nested.svelte...

--->



<!--- solution --->


<!--- in src/app.svelte --->
<script>
	import Nested from './Nested.svelte';
</script>

<p>This is a paragraph.</p>
<Nested />

<style>
	p {
		color: purple;
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}
</style>


<!--- in src/Nested.svelte --->
<p>This is another paragraph.</p>

