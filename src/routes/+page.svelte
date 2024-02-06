<script>
    import {setlist} from '../../data.js';
    
</script>

<div id="setListContainer">
    <ul>
        {#each setlist as song, index }
        <li>
            <p style='color: white'>{song.song} - {song.artist}</p>
        </li>
        <br />
        {/each}
    </ul>
</div>

<style>
    #setListContainer {
        border: white 2px solid;
        margin-left: 10vw;
        margin-right: 10vw;
    }
</style>
