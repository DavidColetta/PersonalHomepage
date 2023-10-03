<script>
  import Header from '../../header.svelte';
</script>

<Header />

<div id="BodyText">
  <h3>> Projects</h3>
  <p>> <a href="https://devpost.com/software/solar-roulette" target="_blank">Solar Roulete (HackRPI 2022 Winner)</a><br>
  An educational website which gives users a sense of the scale of our solar system. Pulls data from an API. Made in one weekend as part of the HackRPI 2022 hackathon, where it won 2nd place overall.</p>
  <p>> <a href="https://chickoonlord.itch.io/space-defense" target="_blank">Space Defense</a><br>
  A tower defense game made in Unity and uploaded to itch.io. This is one of my oldest projects. Be warned, it is a difficult game.</p>
  <p>> <a href="https://infomatrix.cyclic.app/" target="_blank">Infomatrix</a><br>
  An information management system made with NodeJS and MongoDB. Make an account and store information in the form of blogs.</p>
  <p>> <a href="https://davidcoletta.github.io/PersonalWebsite/ResumeBuilder/index.html" target="_blank">Resume Builder</a><br>
  Made as my class project for Intro to ITWS at RPI, this is a resume generation website. Just input your information and dynamically update the form with jquery, then submit and view your compiled resume.</p>
</div>

<style> 
  #BodyText {
    font-size: 1.1em;
  }
  a {color:rgb(0, 183, 255); }
</style>