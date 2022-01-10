<template>

    <div class="select_bar">
        <select @change="$emit('genreSelection',SelectValue)" v-model="SelectValue" class="form-select " name="" id="">
            <option selected>Choose</option>

            <option value="Rock">Rock</option>
            <option value="Pop">Pop</option>
            <option value="Jazz">Jazz</option>
            <option value="Metal">Metal</option>

        </select>  
        
    </div>
    
</template>


<script>
export default {
    name:'SelectBar',

    data:function(){
        return{
            SelectValue:'',
            

        };
    },
    // end data

   
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.select_bar{
    margin-top:10px;
    margin-bottom: 20px;
    
        select{
        padding:5px;
        color:$brand-text-color;
        
        
    }
}

    

</style>