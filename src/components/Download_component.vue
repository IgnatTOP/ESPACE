<template>
    <div class="download_container">
        <p class="title">Скачать игру</p>
        <div class="download">
            <p class="titlePod">Минимальные характеристики:</p>
            <ul>
                <li>ОС: Windows 7, 8, 10, macOS</li>
                <li>Оперативная память: 4 GB ОЗУ</li>
            </ul>
            <div class="buttons">
                <div class="button_title">
                    <p class="windows">Windows</p>
                    <div class="button_download"><p class="download_button">Скачать</p></div>
                </div>
                <div class="button_title">
                    <p class="macos">MacOS</p>
                    <div class="button_download"><p class="download_button">Скачать</p></div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Download_Component',
    components: {
    },

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
.download_container{
    max-width: 80%;
    margin: 0 auto;
}
.titlePod{
    margin: 10px 0 25px;
}
.button_download{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background: #C1EEF8;
    border-radius: 25px;
    width: 379px;
    height: 84px;
    margin: 0 60px 100px;
}
.windows{
    margin: 50px 0 10px 0;
}
.macos{
    margin: 50px 0 10px 0;
}
ul{
    margin: 0;
}
.download_button{

    font-family: 'Jura';
    font-style: normal;
    font-weight: 600;
    font-size: 48px;
    line-height: 57px;
    color: #000000;
}
.download{
    display: flex;
    font-family: 'Jura';
    font-style: normal;
    font-weight: 600;
    font-size: 64px;
    line-height: 76px;
    text-align: center;
    background-color: rgba(0, 0, 0, 0.86);
    color: #FFFFFF;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
.buttons{
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>