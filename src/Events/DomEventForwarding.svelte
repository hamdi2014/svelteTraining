<script>
    import CustomeButton from "./CustomeButton.svelte";

    function handleClick() {
        alert('Button Clicked')
    }
</script>

<CustomeButton on:click={handleClick}/>