<template >
    <div class="card col-2 p-0  " style="border-radius: 0;" >
       <img :src="image" class="card-img-top" alt="picture">
       <div class="card-body text-center">
        <h5 class="card-title">{{name}}</h5>
        <p class="card-text">{{ archetype }}</p>
       </div>
    </div>
    
    
    
</template>

<script>
export default {
    name:'CardComic',
    data(){
        return {

        }
    },
    props:{
         image : String,
         name : String,
        archetype : String,
    }
   
}
</script>

<style lang="scss" scoped>
.card{
    width: calc((100% / 5) - .8rem);
    margin: .4rem ;
    object-fit: cover;
}
  
</style>