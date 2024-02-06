<script>
    export let headerText = 'Welkom bij de donderJam!';
    import {page} from '$app/stores';
    $: url = $page.url; 
</script>

<header>
    {#if url.pathname == '/'}
        <h1>{headerText}</h1>
    {:else}
        <h1>{url.pathname.slice(1)}</h1>
    {/if}
    <nav>
        <ul>
            <li><a href="/info">Info</a></li>
            <!--
            <li><a href="/meedoen">Ik wil meedoen</a></li>
            <li><a href="/aandragen">Ik weet een leuk nummer</a></li>
            -->
        </ul>
        
    </nav>
</header>

<slot />

<style>
    
    header {
        text-align: center;
        background-color: black;
        color: white;
    }
    nav ul {
        display: flex;
        flex-wrap: wrap;
        list-style-type: none;
        justify-content: space-between;
    }

    a {
        text-decoration: none;
        color: white;
    }
    
    
</style>