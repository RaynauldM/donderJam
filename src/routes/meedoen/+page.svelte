<script>
    import Thuis from "../../components/Thuis.svelte" 
</script>

<Thuis />

<form method="POST">
    <label>
        Naam
        <input name='meedoenNaam' type='text' >
    </label>
    <label>
        Instrument
        <input name='instrument' type='checkbox'>
    </label>
    <label>
        Nummer en artiest
        <input name='meedoenNummerEnArtiest' type='text'>
    </label>
    <label>
        Welke donderjam
        <input name='datum' type='checkbox'>
    </label>
    <label>
        email
        <input name='meedoenEmail' type='email'>
    </label>
</form>