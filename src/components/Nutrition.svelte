<script>
    import { nutrition } from '../componentsData/data';
</script>

<section>
    <h2>Nutrition</h2>
    <p>The table below shows nutritional values per serving without the additional fillings.</p>
    
    <div>
        {#each nutrition as val}
            <div>
                <span>{val.nutrient}</span>
                <strong>{val.value}</strong>
            </div>
        {/each}
    </div>
</section>


<style>
    section{
        padding-top: 2em;
    }
    h2{
        margin-bottom: 1em;
    }

    section > div {
        margin-block: 1.5em;
    }

    div > div{
        display: flex;
        justify-content: space-between;
        padding-inline: 3em;
        gap: 2em;
        align-items: center;
        margin-block: 1em;
        padding-bottom: 1em;
        border-bottom: 1px solid var(--neu-light-grey);
    }

    div > div:last-child{
        border-bottom: none;
        margin-bottom: 0;
    }

    div > div strong{
        color: var(--primary-nutmeg)
    }

    
	@media (min-width:40em){
        div > div{
          display: grid;
          grid-template-columns: 1fr 1fr;
        }
	}
</style>