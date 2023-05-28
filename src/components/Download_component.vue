<template>
    <div class="download_container">
        <p class="title">Скачать игру</p>
        <div class="download">
            <p class="titlePod">Минимальные характеристики:</p>
            <ul class="pc">
                <li>ОС: Windows 7, 8, 10, macOS</li>
                <li>Оперативная память: 4 GB ОЗУ</li>
            </ul>
            <p class="mobile">ОС: Windows 7, 8, 10, macOS</p>
            <p class="mobile">Оперативная память: 4 GB ОЗУ</p>
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
.mobile{
    display: none;
    margin: 0;
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
@media (max-width: 600px) {
    .title{
        font-size: 64px;
        line-height: normal;
        margin: 50px 0 30px;
        text-align: center;
    }
    .download{
        font-size: 32px;
        line-height: 46px;
    }
    .button_download{
        border-radius: 15px;
        width: 170px;
        height: 55px;
        margin: 0 10px 65px;
    }
    .download_button{
        font-size: 28px;
    }
    .pc{
        display: none;
    }
    .mobile{
        display: block;
    }
}

</style>