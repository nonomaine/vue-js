<template>
<div>
    <ul class="liste mt-5">
        <li v-for ="(film, index) in myArr" v-bind:key="index"> 
            <div class="card">
                <div class="card-body">
            Titre: {{ film.titre }}
            <br>
            Date: {{ film.date }}

                </div>
            </div>

        </li>
    </ul>
    <div v-on:click="supprFilm" class="btn btn-danger">supprime le film</div>

</div>
</template>

<script>


export default {
    name: 'listeFruit',
    data(){
        return{
            fruits: ['orange', 'papaye', 'fraise']
        }
    },
    methods:{
        supprFilm: function(){
           this.myArr.pop()
        }

    },
    props: ['myArr']
    }
   



</script>

<style scoped src="./liste.css">

</style>
