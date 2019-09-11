<template>
  <svg 
    width="600" 
    height="600" 
    viewBox="0 0 250 250" 
    xmlns="http://www.w3.org/2000/svg">
    <filter id="turbulence">
      <feTurbulence 
        type="turbulence" 
        id="turbulenceFilter" 
        baseFrequency="0.20" 
        numOctaves="5" 
        result="turbulence"
         ></feTurbulence>
      <feDisplacementMap
        in2="turbulence"
        id="displacementFilter" 
        in="SourceGraphic"
        scale="25"
        xChannelSelector="B"
        yChannelSelector="G"
      ></feDisplacementMap>
      
      <animate 
        xlink:href="#turbulenceFilter"
        id="animate1" 
        attributeName="baseFrequency"
        begin="0;animate2.end"
        from="0.20"
        to="0.40"
        dur="5s"
      />
      
      <animate 
        xlink:href="#turbulenceFilter"
        id="animate2" 
        begin="animate1.end"
        attributeName="baseFrequency"
        from="0.40"
        to="0.20"
        dur="5s"
      />
    </filter>
    <rect 
      width="225" 
      height="150" 
      fill="blue" 
      filter="url(#turbulence)"/>

    <foreignObject 
      x="5%" 
      y="10%" 
      width="90%" 
      height="90%">
      <div style="color:red" xmlns="http://www.w3.org/1999/xhtml">
        <slot>
          <p>The HTML works..</p>
        </slot>
      </div>
    </foreignObject>
  </svg>
</template>

<script>
export default {};
</script>

<style scoped>
</style>
