<div class="typing-container">
  <span id="sentence" class="sentence"><slot/></span>
  <span class="input-cursor"></span>
</div>

<style>
  .typing-container {
      display: flex;
      justify-content: center;
      align-items: center;
}
 .input-cursor {
      display: inline-block;
      width: 2px;
      height: 42px;
      background-color: white;
      margin-left: 8px;
      animation: blink .6s linear infinite alternate;
}

@keyframes blink {
    0% {opacity: 1;}
    40% {opacity: 1;}
    60% {opacity: 0;}
    100% {opacity: 0;}
  }
</style>