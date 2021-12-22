<template>
    <div class="main-card">
        <div class="row">
            <!-- SINGLE CARD -->
              <div class="single_card">
                  <div class="my_banner">
                      <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">

                      <div class="banner_title">
                          <h2>TITOLO</h2>
                          <h3>author</h3>
                          <h3>year</h3>
                      </div>
                  </div>
              </div>
          </div>
    </div>
</template>

<script>
export default {
    name:'SingleAlbum',

}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.single_card{
    width: calc(100% / 6);
    margin:30px;
    min-height: 350px;
    
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