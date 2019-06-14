<template>
  <div>
    <h2>HELLO {{name}}</h2>
    <ul>
      <li>Age: {{age}}</li>
      <li>Color: {{color}}</li>
      <li>{{ treat }}</li>
    </ul>
  </div>
</template>  
<script>
export default {
  props: ["treat"],
  data: function() {
    // what value want to receive from the parent in App.vue,"treat" become Proporty, call above in the <template>

    return {
      name: "Simba",
      age: 6,
      color: "black"
    };
  }
};
</script>  
<style >
h2 {
  color: coral;
}
</style>