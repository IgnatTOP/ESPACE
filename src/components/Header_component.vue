<template>
    <div class="main_container" v-on:mousemove="moveDiv">
        <img src="../img/racketa.svg" class="raketa" :style="divStyle">
        <p class="title_name">ESPACE</p>
        <img src="../img/tarelka.svg" class="tarelka" :style="divStyle">
        <div class="buttons">
            <div class="button_pod" @click="scroll2"><p class="text_button">Подробнее</p></div>
            <div class="button_down" @click="scroll4"><p class="text_button">Скачать игру</p></div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Header_Component',
    components: {
    },
    data() {
        return {
            mouseX: 0,
            mouseY: 0,
            maxOffset: 20,
        };
    },
    computed: {
        divStyle() {
            const offsetX = (this.mouseX / window.innerWidth - 0.5) * 2 * this.maxOffset;
            const offsetY = (this.mouseY / window.innerHeight - 0.5) * 2 * this.maxOffset;

            return {
                transition: 'transform 0.3s ease-out',
                transform: `translate3d(${offsetX}px, ${offsetY}px, 0)`,
            };
        }
    },
    methods: {
        moveDiv(event) {
            // обновляем положение мыши
            this.mouseX = event.clientX;
            this.mouseY = event.clientY;
        },
        scroll4(){
            this.$emit('scroll4')
        },
        scroll2(){
            this.$emit('scroll2')
        },
    }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Concert+One&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Concert+One&family=Jura:wght@300;400;500;600;700&display=swap');
.title_name{
    font-family: 'Concert One';
    font-style: normal;
    font-weight: 400;
    font-size: 188px;
    background-color: #4370f0d9;
    color: transparent;
    text-shadow: 0px -6px 0px #ffffff;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    background-clip: text;
}
.tarelka{
    position: absolute;
    margin-left: auto;
    margin-right: auto;
    left: 911px;
    right: 0;
    margin-top: -156px;
    text-align: center;
}
.text_button{
    color: #303264;
    font-family: 'Jura';
    font-style: normal;
    font-weight: 600;
    font-size: 48px;
    text-shadow: 0px 4px 4px rgba(51, 70, 236, 0.25);
}
.raketa{
    position: absolute;
    margin-left: auto;
    margin-right: auto;
    left: 0;
    right: 1037px;
    margin-top: -273px;
    text-align: center;
}
.button_pod, .button_down{
    display: flex;
    justify-content: center;
    align-items: center;
    background: #C1EEF8;
    border-radius: 25px;
    width: 380px;
    height: 85px;
    margin: 107px 60px 0;
    cursor: pointer;
}
.buttons{
    display: flex;
    align-items: center;
    justify-content: center;
}
@media (max-width: 600px) {
   .tarelka{
       margin-top: -38px;
       left: 280px;
       width: 110px;
   }
    .button_pod, .button_down{
        border-radius: 15px;
        width: 160px;
        height: 48px;
        margin: 25px 13px 0;
    }
    .title_name{
        display: flex;
        align-items: center;
        justify-content: center;
        margin: 80px 0 50px;
        font-size: 86px;
    }
    .text_button{
        font-size: 22px;
    }
    .raketa{
        width: 97px;
        right: 256px;
        margin-top: -71px;
    }
}
</style>