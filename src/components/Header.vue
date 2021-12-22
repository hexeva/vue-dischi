<template>
   <header>
       <div class="logo">
           <img src="../assets/img/spotify.png" alt="logo spotify">
       </div>
   </header>
</template>

<script>
export default {
    
    name:'Header',
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

    header{
        width: 100%;
        padding: 14px 20px;
        
        background-color:$brand-primary-color;

        .logo{
            width: 45px;
            height: auto;
            border-radius: 50%;
            overflow: hidden;
            background-color: $brand-primary-color;
            
          
            
            
        }
    }

</style>