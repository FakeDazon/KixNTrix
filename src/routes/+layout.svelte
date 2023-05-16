<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import "$lib/app.css"
    import "$lib/font.css"
</script>

<Header></Header>
<main><slot></slot></main>

<Footer></Footer>

<style>
    main {
        padding-top: 70px;
    }
</style>