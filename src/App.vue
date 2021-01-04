<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
              <button @click="selectedComponent = 'ComponentOne'" class="btn btn-info">One</button>
              <button @click="selectedComponent = 'ComponentTwo'" class="btn btn-danger" >Two</button>
              <button @click="selectedComponent = 'ComponentThree'" class="btn btn-primary" >Three</button>
               <quote>
                 <h1 slot="heading1">hello h1 quote</h1>
                 <h2 slot="heading2" >hello h2 quote</h2>
                  <h1 slot="heading2">Hai h1 quote</h1>
                 <h2 slot="heading1" >Hai h2 quote</h2>
               </quote>
               <component :is='selectedComponent'></component>
            </div>
        </div>
      <!-- <QuotationGrid :quotes = "quotes"></QuotationGrid> -->
    </div>
</template>

<script>
import Quote from './components/Quote.vue';
import ComponentOne from "./components/CompoOne";
import ComponentTwo from "./components/compoTwo";
import ComponentThree from "./components/compoThree";

//----------------------------------
//import QuotationGrid from "./components/project/QuotationGrid.vue";
    export default {
        components:{
          Quote,
          ComponentTwo,
          ComponentOne,
          ComponentThree
          // QuotationGrid
        },
    data(){
      return{
        selectedComponent:'ComponentTwo',
        //----------------------------------
       // quotes:['the quote here']
      }
    }
    }
</script>

<style >
 

</style>
