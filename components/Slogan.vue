<template>
<div class="slogan-container">
    <h1 class="slogan">
        <span>Building</span> <br>
        <span>The</span>
        <span class="neonText">Websites</span>
        <span>&</span>
        <span  class="neonText">Apps,</span>
        <span>You've</span> <br>
        <span>Always</span>
        <span  class="neonText">Dreamed</span>
        <span>Of</span>
    </h1>

    <img class="slogan-logo" src="~/assets/jc.svg" alt="j_logo">
</div>
</template>

<script>
export default {

}
</script>

<style>

* {
  padding: 0;
  margin: 0;
}

.slogan-container{
    display: flex;
    justify-content: center;
    align-items: center;
}

.neonText {
    font-weight: bolder;
  color: #fff;
  text-shadow:
      0 0 2px #fff,
      0 0 4px #fff,
      0 0 8px #fff,
      0 0 16px #0fa,
      0 0 21px #0fa,
      0 0 42px #0fa,
      0 0 84px #0fa,
      0 0 138px rgb(0, 174, 255);
}

.slogan-logo{
    
    opacity: 0;
    filter: blur(4px);
    transition: 0.4s;
    /* transform: scale(0.94); */
    /* animation: scale 3s forwards cubic-bezier(0.5, 1, 0.89, 1); */
    position: absolute;
    left: 50%;
    width: 400px;
    margin-left: -230px;
    transform: scale(0.80);
}

.slogan-container:hover .slogan-logo{
    transform: scale(1);
    opacity: 1;
    filter: blur(0px);
}

.slogan {
    font-size: calc(6px + 2vw);;
    transition: 0.4s;
    /* font-size: xx-large; */
  max-width: 900px;
  /* text-align: center; */
  transform: scale(0.94);
  animation: scale 3s forwards cubic-bezier(0.5, 1, 0.89, 1);
  position: absolute;
  position: absolute;
    left: 50%;
    width: 900px;
    margin-left: -450px;
}


.slogan-container:hover .slogan{
transform: scale(0.94);
  opacity: 0;
  filter: blur(4px);
}

@keyframes scale {
  100% {
    transform: scale(1);
  }
}

.slogan span {
  display: inline-block;
  opacity: 0;
  filter: blur(4px);
}

.slogan span:nth-child(1) {
  animation: fade-in 0.8s 0.1s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(2) {
  animation: fade-in 0.8s 0.2s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(3) {
  animation: fade-in 0.8s 0.3s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(4) {
  animation: fade-in 0.8s 0.4s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(5) {
  animation: fade-in 0.8s 0.5s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(6) {
  animation: fade-in 0.8s 0.6s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(7) {
  animation: fade-in 0.8s 0.7s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(8) {
  animation: fade-in 0.8s 0.8s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(9) {
  animation: fade-in 0.8s 0.9s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(10) {
  animation: fade-in 0.8s 1s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(11) {
  animation: fade-in 0.8s 1.1s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(12) {
  animation: fade-in 0.8s 1.2s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(13) {
  animation: fade-in 0.8s 1.3s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(14) {
  animation: fade-in 0.8s 1.4s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(15) {
  animation: fade-in 0.8s 1.5s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(16) {
  animation: fade-in 0.8s 1.6s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(17) {
  animation: fade-in 0.8s 1.7s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

.slogan span:nth-child(18) {
  animation: fade-in 0.8s 1.8s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

@keyframes fade-in {
  100% {
    opacity: 1;
    filter: blur(0);
  }
}
</style>