<template>
  <svg 
    width="600" 
    height="600" 
    viewBox="0 0 250 250" 
    xmlns="http://www.w3.org/2000/svg">
    <filter id="turbulence">
      <feTurbulence 
        type="turbulence" 
        baseFrequency="0.20" 
        numOctaves="2" 
        result="turbulence"></feTurbulence>
      <feDisplacementMap
        in2="turbulence"
        in="SourceGraphic"
        scale="25"
        xChannelSelector="R"
        yChannelSelector="G"
      ></feDisplacementMap>
    </filter>
    <rect 
      width="225" 
      height="150" 
      fill="blue" 
      filter="url(#turbulence)"/>
  </svg>
</template>

<script>
export default {
};
</script>

<style scoped>
</style>
