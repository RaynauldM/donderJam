<script>
    const allowedNames = [
        'raynauld',
        'jur',
        'david',
        'peter'
    ]
    $: loggedIn = '';
    $: name = '';
    function handleSubmit(event) {
        event.preventDefault();
        if (allowedNames.includes(name)) {
            loggedIn = 'true'
        }
    }
</script>

<h1>Huisband pagina</h1>



{#if loggedIn == ''}
    <form on:submit={handleSubmit}>
        <label>
            Naam:
            <input type='text' bind:value={name}>
        </label>
        <button type='submit'>Let's go!</button>
    </form>
{:else}
    <h2>logged in</h2>
{/if}

<style>
    h2 {
        color: white;
    }
</style>