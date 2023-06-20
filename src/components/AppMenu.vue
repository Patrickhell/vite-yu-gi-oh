<template >
    <main>
        <div class="container1">
            <div class="card m-auto" style="border-radius: 0; width: 1300px; ">
              <h2 class="card-header">Yu-Gi-Oh! API</h2>
              <div class="card-body">
                <div class="container2">
                  <div class="card text-white py-5 m-auto " style="border-radius: 0 ; width: 1000px; border: 0;">
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
    margin: 0 auto;
}
div.card-body{
    background-color:#d48f38 ;
   padding-top: 3rem;

}

.container2{
    width: 1100px;
    background: white;
    margin:0 auto;
    margin-top: 3rem
  
    
}

</style>