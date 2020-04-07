<template>
    <div class="container">
        <div class="row max-height align-items-center text-center">
            <div class="col text-center">
                <button class="btn btn-outline-secondary " v-on:click= "changeBackground()">Click Me!</button>
            </div> 

        </div>
               
    </div>
    
</template>

<script>
export default {
  
  data () {
    return {
     colors:['red', 'green', 'yellow', 'black', 'pink', 'violet']
    }
  },
  methods:{
      changeBackground(){
          let colorIndex = parseInt(Math.random() * this.colors.length);
          document.body.style.backgroundColor = this.colors[colorIndex]
          
      }
  }
}
</script>

<style>
button {
    margin-top: 50vh;
    
}
</style>
