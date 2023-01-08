<!--- new --->

<script>
	let count = 0;

	function increment() {
		// event handler code goes here
	}
</script>

<button>
	Clicked {count}
	{count === 1 ? 'time' : 'times'}
</button>


<!--- 

At the heart of Svelte is a powerful system of reactivity for keeping the DOM in sync with your application state — for example, in response to an event.

To demonstrate it, we first need to wire up an event handler (we'll learn more about these later)

Inside the increment function, all we need to do is change the value of count
--->

<!--- solution --->
<script>
	let count = 0;

	function increment() {
		count += 1;
	}
</script>

<button on:click={increment}>
	Clicked {count}
	{count === 1 ? 'time' : 'times'}
</button>

