<template >
    <main>
        <div class="container1">
            <div class="card " style="border-radius: 0">
              <h2 class="card-header">Yu-Gi-Oh! API</h2>
              <div class="card-body">
                <div class="container2">
                  <div class="card text-white p-4 " style="border-radius: 0 ">
                    <p class="card-header" style="background-color:black;border-radius: 0; height: 50px;">Found 39 cards</p>
                    <div class="card-body p-0" style="background-color: white; " >
                        <CardsList />
                    </div>
                  </div>
                </div>
              </div>
            </div>
        </div>
    </main>
</template>
<script>
import CardsList from './CardsList.vue';

export default {
    name:'AppMain',
    data(){
        return {

        }
    },
     components:{
        CardsList,
     }
    
}
</script>
<style lang="scss">
.container1{
    width: 1000px;
    margin: 0 auto;
    padding-top:1rem;
}
div.card-body{
    background-color:#d48f38 ;
   padding-top: 3rem;

}

.container2{
    width: 900px;
    background: white;
    margin:0 auto
  
    
}

</style>