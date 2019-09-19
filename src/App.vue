<template>
  <div id="app">
<!--     
    Basic Shape:<br/>
    <basicShape></basicShape>
    -->
    <!--     
    Shape with filter: <br/>
    <shapeWithFilter></shapeWithFilter>
    -->
<!--     
    Foreing Object:<br/>
    <foreignObject></foreignObject>
    -->
    

    <!-- With Animation:<br/>
    <componentWIthAnimation>
      <img src="./assets/logo.png" width="25px" height="25px" alt="Example logo">
      <h1>Lets move!</h1>
    </componentWIthAnimation
    -->
<!--     
    Final component:<br/>
    <finalComponent>
      <img src="./assets/logo.png" width="25px" height="25px" alt="Example logo">
      <h1>My heading</h1>
    </finalComponent> -->

<!--     
    Final component with props set:<br/>
    <finalComponent :animate="true" :filter="true">
      <img src="./assets/logo.png" width="25px" height="25px" alt="Example logo">
      <h1>My heading</h1>
    </finalComponent> -->
  </div>
</template>

<script>
import basicShape from "./components/1.basicShape";
import shapeWithFilter from "./components/2.shapeWithFilter";
import foreignObject from "./components/3.foreignObject";
import componentWIthAnimation from "./components/4.componentWIthAnimation";
import finalComponent from "./components/5.finalComponent";

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
