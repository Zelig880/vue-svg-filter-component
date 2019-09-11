<template>
  <div id="app">
    <!-- 
    Basic Shape:
    <basicShape></basicShape>
    -->
    <!--     
    Shape with filter: 
    <shapeWithFilter></shapeWithFilter>
    -->
    <!--
    Foreing Object:
    <foreignObject></foreignObject>
    -->
    <!--
    Final component:
    <finalComponent>
      <img src="./assets/logo.png" width="25px" height="25px" alt="Example logo">
      <h1>My heading</h1>
    </finalComponent> -->
    <!--
    With Animation:
    <componentWIthAnimation>
      <img src="./assets/logo.png" width="25px" height="25px" alt="Example logo">
      <h1>Lets move!</h1>
    </componentWIthAnimation> 
    --> 
  </div>
</template>

<script>
import basicShape from "./components/1.basicShape";
import shapeWithFilter from "./components/2.shapeWithFilter";
import foreignObject from "./components/3.foreignObject";
import finalComponent from "./components/4.finalComponent";
import componentWIthAnimation from "./components/5.componentWIthAnimation";

export default {
  name: "App",
  components: {
    basicShape,
    shapeWithFilter,
    foreignObject,
    finalComponent,
    componentWIthAnimation
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 600px;
}
</style>
