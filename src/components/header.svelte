<script>
  import logo from '$lib/maria-logo.svg';
</script>
<div id="nav">
  <img id="logo" src={logo} alt="logo">
</div>
<style>
  #nav {
    position: fixed;
    top: 0;
    bottom: 0;
    z-index: 11;
    background:#ffffff82;
    display: flex;
  }
  #logo {
    width: 2rem;
    height: auto;
    padding: 1rem;
  }
</style>