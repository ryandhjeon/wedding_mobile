<template>
    <div id="snow" class="main__container fade-in">
        <el-image class="main_image" :src="main" fit="cover" loading="lazy"/>
        <div class="main__description">
            The marriage of
        </div>
    </div>
</template>

<script setup>
    import main from "/src/assets/img/main.jpeg"
</script>

<style scoped>
    .main__container {
        position: relative;
        text-align: center;
    }
    .main_image {
        -webkit-filter: grayscale(100%); /* Safari 6.0 - 9.0 */
        filter: grayscale(100%);
    }

    .main__description {
        position: absolute;
        bottom: 10%;
        left: 0;   
        width: 100%;
        margin: 0 auto; 
        color: white;
        text-shadow: 1px 1px 1px #8c8c8c;
        text-transform: uppercase;
        letter-spacing: 0.5em;
        font-weight: bold;
        font-size: 0.8em;
        border-radius: 10em;
    }
</style>

