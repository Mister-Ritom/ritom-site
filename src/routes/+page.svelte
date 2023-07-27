
<script lang="ts">
    import image from "../components/myImage.png";
    import AnonMedia from "../components/images/logo_anonmedia.png"
    import Anons from "../components/images/logo_anons.png"
    import Unnet from "../components/images/logo_unnet.jpg"
    import Ananta from "../components/images/logo_ananta.png"
    import Project from "../components/project.svelte";
    import Github from "../components/icons/github.png"
	import { onMount } from "svelte";


</script>

<div class="image-container">
    <img class="myImage" src={image} alt="me in a suit"/>
</div>
<h1>Ritom Ghosh</h1>
<p>Journey of My software engineering</p>
<h3>Learning languages:  </h3>
<ul class="languages">
    <li class="language"><p >C++</p></li>
    <li class="language"><p >Java</p></li>
    <li class="language"><p >Kotlin</p></li>

</ul>

<h3>Projects</h3>
<ul class="projects">
    <li><Project name="AnonMedia" logo={AnonMedia} 
        desc="A social media app that collects only minimum data"/></li>
    <li><Project name="Anons" logo={Anons} 
        desc="Anonmedia for brower and desktop (not finished yet)"/></li>
    <li><Project name="Unnet" logo={Unnet} 
        desc="A futuristic social media app with all social media functionality and more"/></li>
    <li><Project name="Ananta" logo={Ananta} 
        desc="Minecraft utility mod using fabric in java"/></li>
</ul>
<h2 class="github-sponsor">Checkout my other projects at
     <a href="https://github.com/ritomg69" target="_blank">Github <img src={Github} alt="Github icon"/></a></h2>
<p></p>

<style>

    @import url("https://fonts.googleapis.com/css?family=Quicksand:400,700");

    .image-container{
        aspect-ratio: 1 / 1;
        display: block;
        margin-left: auto;
        margin-right: auto;
        width: fit-content;
        height: fit-content;
        border-style: solid;
        border-width: 5px;
        border-color:var(--primary);
        border-radius: 50%;
        overflow: hidden;
    }
    .myImage {
        width: 24rem;
        height: 24rem;
    }
    .projects {
        list-style: none;
        display: grid;
        width: max-content;
        row-gap: 16px;
        column-gap: 10px;
        grid-template-columns: 1fr 1fr;
        grid-auto-flow: row;
    }
    .languages {
        display: flex;
        width: fit-content;
        list-style-type: none;
    }
    .language {
        color: white;
        font-family: "Poppins";
        background-color: var(--secondary);
        padding-left: 16px;
        padding-right: 16px;
        padding-top: 8px;
        padding-bottom: 3px;
        margin: 16px;
        border-radius: 16px;
        transition: 1s;
    }
    .language:hover{
        scale:1.3;
        color: var(--accent);
    }
    .github-sponsor{
        margin-left: 16px;
    }

</style>
