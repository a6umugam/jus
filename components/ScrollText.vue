<template>
    <div id="scroll-container">
        <div id="scroll-text" v-if="isFr"><p>Construire les sites Web et les applications dont vous avez toujours rêvé. Nous créons des sites Web professionnels, beaux et uniques pour les petites et grandes entreprises.</p><div></div></div>
        <div id="scroll-text" v-else ><p>Building the <strong>Websites</strong>  & <strong>Apps</strong>, You've Always <strong>Dreamed</strong> of. We create <strong>professional, beautiful</strong> and <strong>unique</strong> website designs for small to large businesses.</p><div></div></div>
    </div>
</template>

<script>
export default {
    props:{textData:'',altText:'',isFr:false},
}
</script>

<style>
#scroll-container {
  /* border: 3px solid black; */
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
  background: linear-gradient(90deg, rgba(0,239,255,1) 0%, rgba(72,255,128,1) 100%);
  width: 100%;
  height: 60px;
  font-size: x-large;
}

#scroll-text {
  /* animation properties */
  -moz-transform: translateX(100%);
  -webkit-transform: translateX(100%);
  transform: translateX(100%);
  min-width: 2100px;
  -moz-animation: my-animation 45s linear infinite;
  -webkit-animation: my-animation 45s linear infinite;
  animation: my-animation 45s linear infinite;
}

/* for Firefox */
@-moz-keyframes my-animation {
  from { -moz-transform: translateX(100%); }
  to { -moz-transform: translateX(-100%); }
}

/* for Chrome */
@-webkit-keyframes my-animation {
  from { -webkit-transform: translateX(100%); }
  to { -webkit-transform: translateX(-100%); }
}

@keyframes my-animation {
  from {
    -moz-transform: translateX(100%);
    -webkit-transform: translateX(100%);
    transform: translateX(100%);
  }
  to {
    -moz-transform: translateX(-100%);
    -webkit-transform: translateX(-100%);
    transform: translateX(-100%);
  }
  
  }
</style>