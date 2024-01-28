<script>
    import Thuis from "../../components/Thuis.svelte" 
</script>



<nav>
    <Thuis />
    <ul>
        <li>
            <a href="#introductieContainer">introductie</a>
        </li>
        <li>
            <a href="#regelsContainer">regelementen</a>
        </li>
        <li>
            <a href="#socialsContainer">socials</a>
        </li>
    </ul>
</nav>
<div id="textContainer">
    <div id="introductieContainer" class="container">
        <p>default introductie</p>
    </div>
    <div id="regelsContainer" class="container">
        <p>default regels text</p>
    </div>
    <div id="socialsContainer" class="container">
        <p>default links to socials</p>
    </div>
</div>

<style>
    .container {
        border: solid black 2px;
        margin-bottom: 20em;
    }
</style>