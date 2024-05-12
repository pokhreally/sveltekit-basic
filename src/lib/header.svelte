<script>
    export let title
</script>

<header>
    <div>
        <h1>{title}</h1>
    </div>
    <nav>
        <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/products">Products</a></li>
        <li><a href="/sales">Sales</a></li>
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