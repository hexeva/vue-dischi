<template>
    <div class="main-app">
        <div class="container">
            <SelectBar @genreSelection="chosedGenre" />

            <div v-if="AlbumList.length > 0" class="row row-cols-5">
                <SingleAlbum v-for="(album,index) in AlbumList" :key="index" :albumObject="album"/>
                
            </div>
            
                <Loader v-else />
            
            
        </div>
      </div>
</template>

<script>

import SingleAlbum from "./SingleAlbum.vue";
import Loader from "./Loader.vue";
import SelectBar from "./SelectBar.vue";



import axios from 'axios';
export default {
    name:'DiscCollection',
    components:{
        SingleAlbum,
        Loader,
        SelectBar,
    },

    data:function(){
        return{
            AlbumList:[],
            searchedGenre:'',

        };
    },
    // end data

    methods:{

        chosedGenre:function(genre){

            this.searchedGenre = genre;
            
        }

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

.main-app{
  background-color:$brand-main-color;
  padding: 40px;
  
  
}



</style>