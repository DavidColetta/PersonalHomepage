<script>
  import Glitch from './glitch.svelte';
  import VCR from './vcr.svelte';
</script>

<a href="/" style="text-decoration: none;">
  <div id="header">
    <h1><VCR>David Coletta</VCR></h1>
    <h2>Web Developer + Programmer + Computer Scientist</h2>
  </div>
</a>

<style>
#header {
  background-color: #21457a;
  padding: 1em;
  padding-bottom: 0.5em;
  text-align: center;
  color: #121820;
  border-radius: 4px;
}
h1 {
  color: #d3f5ff;
  padding: 0.5em;
  margin: 0%;
  background-color: #121820;
  border-radius: 1em;
  background: repeating-linear-gradient(
      0deg,
      #0E0D0E 25%,
      #0E0D0E 50%,
      #171819 50%,
      #171819 75%
    );
  background-size: 10px 10px;
  animation: barberpole 10s linear infinite;
}

@keyframes barberpole {
  100% {
    background-position: 100% 100%;
  }
}
</style>
