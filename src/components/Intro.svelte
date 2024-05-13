<script>
    import { preparationTime } from '../componentsData/data'
</script>

<section class="intro">
    <div class="img-container">
        <img src="./images/image-omelette.jpeg" alt="an omelette"  />
    </div>

    <div>
        <h1>Simple Omelette Recipe</h1>
        <p>  An easy and quick dish, perfect for any meal. This classic omelette combines beaten eggs cooked 
            to perfection, optionally filled with your choice of cheese, vegetables, or meats.
        </p>
    
        <div class="preparation">
            <h2>Preparation time</h2>
            <ul>
                {#each preparationTime as val}
                    <li>{@html val}</li>
                {/each}
            </ul>
        </div>
    </div>
</section>


<style>
    .intro > div:nth-child(2){
        padding-inline: 1.3em;
    }

    .intro .img-container img{
        border-radius: 10px;
    }

    .intro h1{
        margin-block: .8em;
        font-size: 2rem;
        line-height: 35px;
        color: var(--neu-dark-charcoal);
        font-weight: 500;
    }

    .preparation {
        border-radius: 10px;
        background-color: var(--neu-rose-white);
        margin-block: 2em;
        padding: 1.5em;
    }

    .preparation h2{
        font-weight: 500;
        margin-bottom: .5em;
        font-family: "Outfit", sans-serif;
        color: var(--dark-raspberry);
        font-size: 1.25rem;
    }
    .preparation ul{
        margin-left: 1em;
    }
    .preparation li{
        font-weight: 500;
        margin-bottom: .5em;
        padding-left: 1em;
        color: var(--neu-wenge-brown)
    }

    
	@media (min-width:40em){
		.intro h1{
            font-size: 2.3rem;
        }
	}
</style>
