<template>
    <div class="loading">
        <img src="https://cdn.dribbble.com/users/24091/screenshots/882638/metaloader.gif" alt="loading image">
    </div>
</template>

<script>
export default {
    name:'Loader',
}
</script>

<style lag="scss" scoped>
.loading{
    position: absolute;
    top:50%;
    left:50%;
    transform: translate(-50%,-50%);
    
}

</style>