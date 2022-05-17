<script>
import Header from "../components/header.svelte"
import Gallery from "../components/gallery.svelte"
import junio from '$lib/junio.webp'

let paintings = [
  { name: 'Junio', img: junio, style: 'max-width: 40rem;' },
  { name: 'Selva', img: junio },
  { name: 'Otono', img: junio }, 
]
</script>

<Header/>
{#each paintings as { name, img, style }, i}
  <Gallery imgg={img} name={ name } style={ style } />
{/each}