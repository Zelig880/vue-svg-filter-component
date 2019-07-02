<template>
  <div id="ciao">
    <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
      <filter id="blurMe">
        <feTurbulence type="turbulence" baseFrequency="0.05" numOctaves="5" result="turbulence"></feTurbulence>
        <feDisplacementMap
          in2="turbulence"
          in="SourceGraphic"
          scale="4"
          xChannelSelector="R"
          yChannelSelector="G"
        ></feDisplacementMap>
      </filter>
      <polygon points="5,5 195,10 185,185 10,195"></polygon>
      <circle cx="60" cy="60" r="50" fill="green"></circle>

      <g filter="url(#blurMe)">
        <foreignObject x="10" y="30" width="190" height="190">
          <div xmlns="http://www.w3.org/1999/xhtml">
            <slot>ciao</slot>
          </div>
        </foreignObject>
      </g>
    </svg>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<style scoped>
</style>
