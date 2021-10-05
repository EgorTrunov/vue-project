<template>
    <div class="container">
        <div class="confiquration">
            <div class="config__questions">
                <p class="question__text">Осталось вопросов <span class="question__number">1</span> из 3</p>
                <div class="question__menu">
                    <ul class="question__list">
                        <li class="question__item">
                            <img src="@/assets/img/rectangle__menu.svg" alt="">
                        </li>
                        <li class="question__item">
                            <img src="@/assets/img/rectangle__menu.svg" alt="">
                        </li>
                        <li class="question__item">
                            <img class="img" src="@/assets/img/rectangle__menu.svg" alt="">
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <h2 class="title">Соберите свой индивидуальный стол</h2>
        <ConfigTable />
        <button class="button">Следующий вопрос</button>
        <div class="client__order">
            <img src="@/assets/img/client-order-img1.jpg">
            <div class="order__application">
                <h2 class="application__title">Реализуем стол под ваш дизайн проект</h2>
                <h2 class="Rosanthie-text">Design</h2>
                <p class="aplication__text">Подоберите все необходимое для оформления завершенного, гармоничного, стильного и уютного интерьера своей квартиры или дома в одном месте.</p>
                <button class="button btn-order">Оставить заявку<span><img src="@/assets/img/arrow-right.svg" alt="Стрелка вправо"></span></button>
            </div>
            <img src="@/assets/img/client-order-img2.jpg">
        </div>
    </div>
</template>

<script>
import ConfigTable from "./ConfigTable.vue"

export default {
    name: 'Configurator',
    components: ConfigTable
}
</script>

<style scoped>
.title {
    text-align: center;
}

.confiquration {
    max-width: 1100px;
    height: 417px;
    background-image: url("../assets/img/config-img.jpg");
}

.config__questions {
    position: relative;
    top: 325px;
    max-width: 650px;
    margin: auto;
    background: #fff;
    padding-top: 30px;
    padding-bottom: 5px;
}

.question__text {
    font-size: 10px;
    line-height: 13px;
    text-align: center;
    color: #B8B8B8;
}

.question__list {
    display: flex;
    justify-content: center;
}

.question__item {
    cursor: pointer;
}

.question__item:not(:last-of-type) {
    margin-right: 40px;
}

.img:hover {
    fill: #000000;
}

.button {
    margin: 75px auto 80px;
}

.client__order {
    margin: 50px 0 50px;
    display: flex;
    justify-content: space-between;
}

.order__application {
    max-width: 410px;
}

.application__title {
    margin: 25px auto;
    font-family: "Kudryashev Display";
    font-size: 60px;
    font-weight: 300;
    line-height: 75px;
}

.btn-order {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 300px;
    padding: 10px;
    margin: 60px 0;
    text-align: center;
}

.btn-order span{
    height: 44px;
    margin-left: 20px;
}

.Rosanthie-text {
    position: relative;
    top: -170px;
    left: 145px;
    line-height: 0;
    margin: 0;
}
</style>