<script>
	import NewProduct from "./NewProduct.svelte";
	export let name;
</script>

<style>
	h1 {
		color: deepskyblue;
	}
</style>

<h1>Hello {name}!</h1>


<section>
<div>
<label for="title">Title</label>
<input type="text" id="title">
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
