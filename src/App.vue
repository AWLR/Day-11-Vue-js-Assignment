<template>
  <div class="container">
  <div id="counter">
      <h1>Vue Js Assignment</h1>
      <p>The Current Count : {{ count }}</p>
     
      <button v-on:click="increment">Increment</button>
      <button v-on:click="decrement">Decrement</button>
      <h2> {{msg}}</h2>
  </div>
</div>
</template>

<script>
export default{

  data() {
      return {
          count: 0,
           msg:null,

      };
  },
  methods: {
      increment() {
          this.count++;
          this.msg= "Counter Increasing";
      },
      decrement() {
          this.count--;
          this.msg= "Counter Decreasing";
      }
  

      },
  }

</script>

<style>
*{
  padding: 10px;
  justify-content: center;
  text-align: center;
}
.container{
  justify-content: center;
}

#counter{
  border: 3px solid greenyellow;
}

button {
background-color: #040aaa; 
margin-right: 5px;
border: none;
color: white;
font-size: 15px;
}
p{
  font-size:larger;
  color: red;
}
</style>


