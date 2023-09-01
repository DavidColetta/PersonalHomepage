<script>
  import Header from '../header.svelte';
  import Glitch from '../glitch.svelte';
  import VCR from '../vcr.svelte';
  import Typing from '../typing.svelte';

  jQuery(function() {
      console.log( "ready!" );
  });


  async function typeSentence(sentence, eleRef, delay = 100) {
    const letters = sentence.split("");
    let i = 0;
    while(i < letters.length) {
      await waitForMs(delay);
      jQuery(eleRef).append(letters[i]);
      i++
    }
    return;
  }


  function waitForMs(ms) {
    return new Promise(resolve => setTimeout(resolve, ms))
  }
</script>

<Header />

<div id="parent">
  <div id="BodyText">
    <h3><Typing>Who am I?</Typing></h3>
    <p>
      Hi! I'm David, a student at Rensselaer Polytechnic Institue dual majoring in <u>Computer Science</u> as well as <u>Information Technology and Web Sciences</u>.<br>
    </p>
    <h3>[ Contacts ]</h3>
    └ Email: davidkcoletta@gmail.com<br>
    └ Discord: chickoon<br>
    └ <a href="https://www.linkedin.com/in/david-coletta-6557a3252/" target="_blank">LinkedIn</a><br>
    └ <a href="https://github.com/DavidColetta" target="_blank">GitHub</a><br>
  </div>
  <div id="BodyText2">
    <h3><a href="/projects">[ Projects ]</a></h3>
    └ <a href="https://devpost.com/software/solar-roulette" target="_blank">Solar Roulete (HackRPI 2022 Winner)</a><br>
    └ <a href="https://chickoonlord.itch.io/space-defense" target="_blank">Space Defense</a><br>
    └ <a href="https://infomatrix.cyclic.app/" target="_blank">Infomatrix</a><br>
    └ <a href="https://davidcoletta.github.io/PersonalWebsite/ResumeBuilder/index.html" target="_blank">Resume Builder</a><br>
  </div>
</div>
<style> 
  #parent {
    margin: 2em;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }
  p {
    margin-bottom: 5em;
  }
  #BodyText {
    font-size: 1.1em;
    width: 40%;
  }
  #BodyText2 {
    font-size: 1.1em;
    width: 50%;
    float: right;
  }
  a {color:rgb(0, 183, 255); }
</style>