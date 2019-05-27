<script>
	import NewProduct from "./NewProduct.svelte";
	
	let title = '';
	let price = 0;
	let description = '';
</script>

<style>
	h1 {
		color: deepskyblue;
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

<h1>Hello {name}!</h1>


<section>
<div>
<label for="title">Title</label>
<input type="text" id="title" value="{title}">
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
