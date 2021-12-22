<template>
    <div class="main-card">
        
            <!-- SINGLE CARD -->
              <div class="single_card">
                  <div class="my_banner">
                      <img :src="albumObject.poster" :alt="albumObject.title">

                      <div class="banner_title">
                          <h2>{{albumObject.title}}</h2>
                          <h3>{{albumObject.author}}</h3>
                          <h4>{{albumObject.year}}</h4>
                      </div>
                  </div>
              </div>
          
    </div>
</template>

<script>
export default {
    name:'SingleAlbum',
    props:{
        albumObject:Object,
    }

}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.single_card{
    
    margin:12px;
    min-height: 400px;
    
    background-color: $brand-primary-color;

    .my_banner{
        width: 100%;
        margin: auto;
        padding: 20px;
    }

    .banner_title{
        text-align: center;
        margin: 20px 0;
        h2{
            margin-bottom: 20px;
        }
        h3{
            margin:unset;
        }

    }
}




</style>