<!--
Adding data
A component that just renders some static markup isn't very interesting. Let's add some data.

First, add a script tag to your component and declare a name variable:
-->


<!--- this outputs: Hello World!--->

<h1>Hello World!</h1>


<!--- this outputs: Hello Svelte! --->
<script>
  let name = 'Svelte';
</script>

<h1>Hello {name}!</h1>


<!--- this outputs: Hello SVELTE! --->
<!--- 
Inside the curly braces, we can put any JavaScript we want. 
Try changing name to name.toUpperCase() for a shoutier greeting.
--->

<script>
  let name = 'Svelte';
</script>

<h1>Hello {name.toUpperCase()}!</h1>

