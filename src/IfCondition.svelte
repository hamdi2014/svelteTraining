<script>
    let user = {loggedIn:false}
    let message;

    function toggle(){
        user.loggedIn = !user.loggedIn;
        message = user.loggedIn ? 'You are logged in!' : 'You are logged out!'
    }
</script>

{#if user.loggedIn}
    <button on:click={toggle}>
        Log in
    </button>
{/if}

{#if !user.loggedIn}
    <button on:click={toggle}>
        Log out
    </button>
{/if}