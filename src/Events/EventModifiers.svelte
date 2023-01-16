<script>
    function handleClick() {
        alert('Clicked');
    }
</script>

<button on:click|once={handleClick}>
    Click me
</button>