<script>
    import {page} from "$app/stores"
    const slugArray = $page.params.slug.split("/");
    
</script>

{#if slugArray.length === 1 && slugArray[0] === ""}
<h1>List of all houses</h1>
{:else if slugArray.length === 1}
<h1>List of houses in {slugArray[0]} area.</h1>
{:else if slugArray.length === 2}
<h1>List of houses in {slugArray[0]} area and under Rs. {slugArray[1]}.</h1>
{/if}