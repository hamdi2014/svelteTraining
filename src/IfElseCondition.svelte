<script>
    let user = {loggedIn:false};
    let message;

    function toggle(){
        user.loggedIn = !user.loggedIn
        message = user.loggedIn ? 'You are Login!' : 'You are Logout!'
    }
</script>

{#if user.loggedIn}
    <button on:click={toggle}>
        Login
    </button>
{:else}
    <button on:click={toggle}>
        Logout
    </button>
{/if}