<script>
    import {page} from "$app/stores"
    const currentPage = $page.url?.pathname
    console.log(currentPage)
    export let title
</script>

<header class="h-[5rem] flex justify-between items-center">
    <div>
        <h1>{title}</h1>
    </div>
    <nav>
        <ul>
        <li class="font-thin hover:font-normal duration-300 w-20 text-center"><a href="/">Home</a></li>
        <li class="font-thin hover:font-normal duration-300 w-20 text-center"><a href="/products">Products</a></li>
        <li class="font-thin hover:font-normal duration-300 w-20 text-center"><a href="/sales">Sales</a></li>
        </ul>
    </nav>
</header>

<style>
    header {
        background-color: #333;
        color: white;
        padding: 1rem;
    }

    nav ul {
        display: flex;
        justify-content: center;
        gap: 1rem;
    }

    nav a {
        color: white;
        text-decoration: none;
    }
</style>