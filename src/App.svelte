<script>
	import NewProduct from "./NewProduct.svelte";
	
	let title = '';
	let price = 0;
	let description = '';

	function setTitle(event) {
		title = event.target.value;
	}
</script>

<style>
	h1 {
		color: cornflowerblue;
	}
	section {
		width: 30rem;
		margin: auto;
	}
	
	label, 
	input,
	textarea {
		width: 100%
	}
</style>

<!--Doesn't output {name} b/c not exported anymore -->
<h1>Hello {name}!</h1> 


<p>{title}</p>
<section>
<div>
<label for="title">Title</label>
<input type="text" id="title" value="{title}" on:input="{setTitle}">
</div>

<div>
<label for="price">Price</label>
<input type="number" id="price">
</div>

<div>
<label for="description">Description</label>
<textarea rows="3" id="description"></textarea>
</div>

</section>

<NewProduct />
