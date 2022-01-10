<template>

    <div class="select_bar">
        <select v-model="SelectValue" class="form-select " name="" id="">
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
    }
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