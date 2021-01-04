<template>
    <div class="row">
        <Quotation v-for="quote in quotes" :key="quote.index">
            {{ quote }}
        </Quotation>
    </div>
</template>

<script>
import Quotation from "./Quotation.vue";
export default {
    props:['quotes'],
    components:{
        Quotation
    }
}
</script>

<style scoped>

</style>