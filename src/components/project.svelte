<script lang="ts">
    export let name:string;
    export let logo:string;
    export let desc:string;
</script>

<div class="parent">
    <div>
        <h1 class="name">{name}</h1>
        <h3 class="desc">{desc}</h3>
    </div>
    <img src={logo} alt={desc}/>

</div>

<style>
    .parent {
        display: flex;
        padding: 10px;
        background-color: var(--secondary);
        border-radius: 32px;
        transition: 1s;
        width: 20rem;
        height:12rem;
    }
    .parent:hover {
        background-color: var(--primary);
        scale: 1.2;
    }
    img {
        width:96px;
        height:96px;
        border-radius: 16%;
        margin:16px;
        margin-top: auto;
        margin-bottom: auto;
    }
    .name {
        text-align: center;
    }
    .desc {
        font-size: medium;
        width: 10rem;
    }
</style>
