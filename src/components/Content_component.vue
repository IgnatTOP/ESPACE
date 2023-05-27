<template>
    <div class="content_container">
            <p class="title">Описание</p>
        <div class="opisanie_container">
            <p>Мы разработали игру Espace
                про астрономию для детей. </p>
            <p>Ребенку будет понятен интерфейс игры.
                Игра носит обучающий характер, но в
                это же время присутствует много игровых
                элементов, благодаря чему детям будет
                легче усваивать новую информацию.  </p>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Content_Component',
    components: {
    }
}
</script>

<style scoped>
.content_container{
    max-width: 80%;
    margin: 0 auto;
}
.title{
    font-family: 'Jura';
    font-style: normal;
    font-weight: 600;
    font-size: 128px;
    line-height: 151px;
    background-color: rgba(0, 0, 0, 0.86);
    color: #FFFFFF;
}
.opisanie_container{
    font-family: 'Jura';
    font-style: normal;
    font-weight: 600;
    font-size: 64px;
    line-height: 76px;
    text-align: center;
    background-color: rgba(0, 0, 0, 0.86);
    color: #FFFFFF;
}
</style>