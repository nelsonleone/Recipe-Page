<script>
    import { ingredients } from '../componentsData/data';
</script>

<section class="ingredients-section">
    <h2>Ingredients</h2>

    <ul>
        {#each ingredients as ingredient}
          <li>{ingredient}</li>
        {/each}
    </ul>
</section>

<style>
    .ingredients-section{
        padding-bottom: 1.5em;
        border-bottom: 1px solid var(--neu-light-grey);
    }
    .ingredients-section h2{
        margin-bottom: .5em;
        font-size: 1.75rem;
    }

    .ingredients-section ul {
        padding-left: 1em;
    }
    
    .ingredients-section li {
        padding-left: 1em;
        margin-bottom: .5em;
    }
</style>