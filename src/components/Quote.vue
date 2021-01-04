<template>
<div>
  <div>
    <!-- <h2>its a quote component</h2> -->
    <slot name="heading1"></slot>
  </div>
  <div>
  <slot name="heading2" ></slot>
  </div>
  </div>
</template>
<script>
export default {};
</script>

<style scoped>
div {
  border: 1px solid #ccc;
  box-shadow: 1px 1px 2px black;
  padding: 30px;
  margin: 30px auto;
  text-align: cente;
}

 h1{
   color: green;
 }

 h2{
   font: outline;
   color: hotpink;
 }

</style>