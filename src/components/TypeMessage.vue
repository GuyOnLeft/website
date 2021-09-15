<template>
  <div class="wrapper">
    <div class="typing-feature">
      Hi. I'm Jeremy. Welcome to my website.
    </div>
  </div>
</template>

<script>
export default {
  name: 'TypeMessage',
  props: {
    msg: String
  }
}
</script>
<style scoped>


.wrapper {
  height: 100vh;
  /*This part is important for centering*/
  display: flex;
  align-items: center;
  justify-content: center;
}

.typing-feature {
  width: 39ch;
  animation: typing 4s steps(39), blink .5s step-end infinite alternate;
  white-space: nowrap;
  overflow: hidden;
  border-right: 3px solid;
  font-family: monospace;
  font-size: 2em;
}

@keyframes typing {
  from {
    width: 0
  }
}

@keyframes blink {
  50% {
    border-color: transparent
  }
}




</style>