<script>
import Header from "../components/header.svelte"
import Gallery from "../components/gallery.svelte"
import junio from '$lib/junio.webp'

let paintings = [
  { name: 'Junio', img: junio },
  { name: 'Selva', img: junio },
  { name: 'Otono', img: junio }, 
]
</script>

<Header/>
{#each paintings as { name, img }, i}
  <Gallery imgg={img} name={name}/>
{/each}