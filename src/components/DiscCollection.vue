<template>
    <div class="main-app">
        <div class="container">
            <SingleAlbum />
        </div>
      </div>
</template>

<script>

import SingleAlbum from "./SingleAlbum.vue";

import axios from 'axios';
export default {
    name:'DiscCollection',
    components:{
        SingleAlbum,
    },

    data:function(){
        return{
            AlbumList:[],

        };
    },

      created:function(){
        axios.get('https://flynn.boolean.careers/exercises/api/array/music')
        .then((response) => {
            // console.log(response.data.response);
            this.AlbumList = response.data.response;

        });

    },

  


}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';



</style>