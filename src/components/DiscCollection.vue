<template>
    <div class="main-app">
        <div class="container">
          <div class="row">
              <div class="single_card">
                  <div class="banner">
                      <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
                  </div>
              </div>
          </div>
        </div>
      </div>
</template>

<script>
import axios from 'axios';
export default {
    name:'DiscCollection',

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