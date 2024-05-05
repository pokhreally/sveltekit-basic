<script>
    import { page } from "$app/stores"
    import { goto, beforeNavigate, afterNavigate } from "$app/navigation"

    const productId = $page.params.productId

    const placeOrder = () => {
        goto("/sales", {replaceState: true})
    }

    beforeNavigate((navigation) => {
        console.log("Executes before navigation", navigation)
    })

    afterNavigate((navigation) => {
        console.log("Executes after navigation for example clicking back button", navigation)})

</script>

<h1>Product page {productId}</h1>
<a href={`/products/${productId}/reviews`}>Reviews</a>

<button on:click={placeOrder}>Place Order</button>