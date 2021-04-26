<script>
	let n = 0;
</script>

<button on:click={() => (n += 1)}>
	clicks: {n}
</button>

<a href="/no-router/a">a</a>
<a href="/no-router/b">b</a>

<slot />

<p>Steps:</p>
<ol>
	<li>Click button, assert clicks = 1</li>
	<li>Go to b, assert clicks = 0</li>
	<li>Click button, assert clicks = 1</li>
	<li>Go to a, assert clicks = 1</li>
	<li>Go to b, assert clicks = 0</li>
</ol>
