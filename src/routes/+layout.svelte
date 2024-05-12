<script>
    import "../app.css";
    import Header from "$lib/header.svelte";
    import Footer from "$lib/footer.svelte";
</script>

<Header title="Svelte"></Header>
<div class="min-h-[calc(100vh-10rem)]">
    <slot></slot>
</div>
<Footer></Footer>

