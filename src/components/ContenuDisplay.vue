<template>
    <div class="container mt-5"> 
    
    <liste v-bind:myArr="myArr"></liste>
    <liste v-bind:myArr="myArr"></liste>

    </div>
</template>

<script>
import liste from'./liste/liste.vue'

export default{
    name: 'ContenuDisplay',
    data(){
        return {
           myArr : [
            {titre: 'Inception', date: 2010},
            {titre: 'Avatar', date: 2009},
            {titre: 'Seven', date: 1995}
           ] 
        }
    },
    components: {
        'liste': liste
    }
}
</script>

<style>

</style>
