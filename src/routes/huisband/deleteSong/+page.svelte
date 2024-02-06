<script>
    import {setlist} from '$lib/data.js'
    
</script>

<div id="setListContainer">
    <ul>
        {#each setlist as song, index }
        <li>
            <button on:click={(event) => {
                let {textContent} = event.target
        if (confirm("Zeker hiervan?")) {
            setlist.splice(index, 1)
        }
            }}>{song.song} - {song.artist}</button>
        </li>
        <br />
        {/each}
    </ul>
</div>

