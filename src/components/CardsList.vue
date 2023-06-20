<template >
    <div class="row justify-content-center " v-if="elementsList.length === 0">
        <div class="col-12 text-center">
          <h1 style="color: black">
            loading comiscCards...
          </h1>

        </div>
        
    </div>
    <div class="row" v-else>
        <CardComic v-for=" cardComic in elementsList"
        :image = 'cardComic.card_images[0].image_url'
        :name = 'cardComic.name'
        :archetype = 'cardComic.archetype' />
    </div> 
</template>

<script>
import CardComic from './CardComic.vue';
import axios from 'axios';

export default {
    name:'CardsList',
    data(){
        return {
            
            elementsList :[],
        }
    },
    components:{
        CardComic,
        
    },
    created(){
        axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0')
  .then((response)=>  {
    // handle success
    console.log(response.data.data);
    setTimeout(()=> {
        this.elementsList = response.data.data
    },2000);

  })
  .catch(function (error) {
    // handle error
    console.log(error);
  })


    }

}
</script>

<style lang="scss" scoped>

</style>