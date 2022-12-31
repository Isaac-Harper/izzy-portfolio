<script>
    /**
	 * @type {string}
	 */
     export let link
</script>



<div class="container">
    <a href={link} class="link">
        <slot></slot>
    </a>
</div>



<style>
    .container {
    }

    .link {
        color: white;
        text-decoration: none;
        padding: 1rem 2rem;
        background-color: #725261;
        border-radius: 2rem;
        
    }

    .link:hover {
        padding: 1.1rem 2.2rem;
    }
</style>