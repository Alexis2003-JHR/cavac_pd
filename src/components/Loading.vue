<template>
    <div class="loading" v-if="isLoading">
        <h3>Loading...</h3>
    </div>
</template>

<script>
export default{
    name: "Loading",
    data(){
      return{
          isLoading: false
      }
    },
    methods: {
    noLoading(){
        setTimeout(() =>{
            this.isLoading = false;
        }, 3000)
    }},
    mounted(){
        let me = this;
        
        this.$root.$on('loadloading', (data) => {
            me.isLoading = data;
        })
    }
}
</script>

<style>
.loading{
    position: absolute;
    display: flex;
    background-color: #000;
    width: 100%;
    height: 100vh;
    color: #fff;
    justify-content: center;
}
</style>