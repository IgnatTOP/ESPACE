<template>
    <div class="Trailer_container">
            <p class="title">Трейлер</p>
        <video controls>
            <source src="../img/IMG_1694.mp4" type="video/mp4">
        </video>
    </div>
</template>
<script>
export default {
    name: 'Trailer_Component',
    components: {
    }
}
</script>

<style scoped>
.title{
    font-family: 'Jura';
    font-style: normal;
    font-weight: 600;
    font-size: 128px;
    line-height: 151px;
    background-color: rgba(0, 0, 0, 0.86);
    color: #FFFFFF;
    margin: 0 0 30px;
}
video{
    width: 720px;
    margin: 0 0 30px;
    border-radius: 10px;
    border: 1px solid white;
}
</style>