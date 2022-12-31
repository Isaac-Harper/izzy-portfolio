<script>
    const size = Math.floor(Math.random() * 5);
    /**
	 * @type {string}
	 */
     export let src

</script>

<div class="container" style="grid-template-columns: {5 - size}fr 5fr {size}fr">
    <div class="space"></div>
    <img {src} alt="lesson">
    <div class="space"></div>
</div>


<style>
    .container {
        display: grid;
        border:  #D3BFC8;
    }
</style>