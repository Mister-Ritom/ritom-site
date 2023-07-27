<script>
    import Footer from "../components/footer.svelte";
</script>

<slot/>
<Footer/>

<style>

  @import url('https://fonts.googleapis.com/css2?family=Kanit&family=Open+Sans:wght@500&family=Poppins:wght@500&display=swap');
    :global(body) {
        --background:#0c0529;
        --text:#d9d1fa;
        --primary:#b843ea;
        --secondary:#450839;
        --accent:#ea43c9;
        overflow-x: hidden;
        background-color:var(--background);
        color:var(--text);
        font-family: "Kanit";
    }

    :global(h3) {
        letter-spacing: 1.5px;
        font-family: "OpenSans";
    }

    :global(a) {
        color: var(--accent);
        text-decoration: none;
    }

</style>