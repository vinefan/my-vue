<template>
    <div class="about">
        <h1>This is an about page</h1>
        <h3>{{name}} : {{msg}}</h3>
    </div>
</template>

<script>

      export default {
            name: "About",
            data(){
                  return{
                        msg: this.$store.state.count,
                        name:this.$store.state.name
                  }
            }
      }
</script>
