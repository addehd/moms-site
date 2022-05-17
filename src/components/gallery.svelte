<script>

export let imgg;
export let style;
console.log(style);

const positions = ["100% 5%", "50% 50%", "00% 00%", "5% 95%", "95% 95%"];
let position = "5% 5%";

let counter = 0
setInterval(() => {
  counter++
  if (counter > positions.length - 1) {
    counter = 0 }
  position = positions[counter]
}, 1500)

</script>


<section class="gallery-image-wrapper">
  <img style="transform-origin: {position}" class="img-zoom" src={imgg} alt="logo">
</section>

<section class="solo-wrapper">
  <img style="{style}" class="img-solo" src={imgg} alt="logo">
  <h1>The answer is</h1>
</section>

<style>
.img-zoom {
  width: 100%;
  transform: scale(140%);
  height: auto; }

/* mobile only query */
@media only screen and (max-width: 600px) {
  .img-zoom {
    width: 200%;
   }
}
.gallery-image-wrapper {
  height: 100vh;
  overflow: hidden;
  max-width: 100vw; }

.solo-wrapper {
  height: 105vh;
  overflow: hidden;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.img-solo {
  width: 80%;
  height: auto; }
</style>
