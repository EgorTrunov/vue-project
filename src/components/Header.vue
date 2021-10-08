<template>
    <div class="container">
        <header class="header">
            <section class="info">
                <nav class="nav-menu">
                    <transition name="fade" mode="out-in">
                       <img class="img-menu" src="@/assets/img/nav.png" width="23" height="23" v-if="!show" @click="show = !show" key="menu">
                       <img class="img-menu" src="@/assets/img/close.png" width="23" height="23" v-else @click="show = !show" key="clear">
                    </transition>
                    <transition mode="fade">
                        <ul class="nav-menu__list" v-if="show">
                            <li class="nav-menu__item" v-for="item in items" :key="item.id">{{ item }}</li>
                        </ul>
                    </transition>
                   
                </nav> 
                <ul class="info-list">
                    <li class="info-item">
                        <h3 class="info-heading city">Москва</h3>
                        <p class="info-text">Ваш город</p>
                    </li>
                    <li class="info-item">
                        <a href="https://goo.gl/maps/RfkjiAV97qoudfUn9" target="_blank">
                            <h3 class="info-heading">Шоурум Artplay</h3>
                            <p class="info-text">Нижняя Сыромятническая, 10с2</p>
                        </a>
                    </li>
                    <li class="info-item">
                        <h3 class="info-heading"><a href="tel:+74950231301">+7 495 023 13 01</a></h3>
                        <p class="info-text">Ежедневно 10:00 - 22:00</p>
                    </li>
                </ul>
                <img src="@/assets/img/search.png" width="30" height="30" id="search"> 
                <img src="@/assets/img/lk.png" width="30" height="30" id="lk">
                <button class="button">Обратный звонок</button>
            </section>
            <section class="nav">
                <img src="@/assets/img/logo.png" width="120" height="52" id="logo">
                <ul class="nav-list">
                    <li class="nav-item">Каталог наличия</li>
                    <li class="nav-item">Информация</li>
                    <li class="nav-item">Мебель на заказ</li>
                </ul>
                <div class="basket">
                    <div id="basket">
                        <img src="@/assets/img/basket.png" width="30" height="30">
                        <img src="@/assets/img/Ellipse.png" width="19" height="19" id="ellipse">
                    </div>
                    <div class="basket-text">
                        <h4 class="basket-heading">Корзина</h4>
                        <p class="basket-sum">18 000₽</p>
                    </div>
                </div>
            </section>
        </header>
    </div>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            items: [
                'Каталог',
                'Информация',
                'Мебель на заказ',
                'Корзина',
                'Контакты'
            ],
            show: false
        }
    }
}
</script>

<style scoped> 

.header {
    font-family: "Geometria";
    font-weight: 400; 
    color: #000000;
    font-size: 16px;
    line-height: 20px;
    margin-top: 35px;
}

ul {
    display: flex;
    justify-content: space-between;
}

.nav-menu {
    padding-top: 5px;
    margin-right: 70px;
}

.info {
    display: flex;
    flex-direction: row;
    margin-bottom: 40px;
}

.info-list {
    width: 540px;
    margin-right: 50px;
}

.info-heading {
    font-family: "Geometria";
    font-weight: 500;
    font-size: 14px;
    line-height: 18px;
    margin: 0;
    margin-bottom: 2px;
}

.info-text {
    color: #9a9a9a;
    font-size: 10px;
    line-height: 13px;
    margin: 0;
}

#search {
    margin-right: 80px;
}

#lk {
    margin-right: 50px;
}

.button {
    margin-top: -10px;
}

.nav {
    display: flex;
}

#logo {
    margin-right: 70px;
}

.nav-list {
    width: 705px;
    margin-right: 100px;
    align-items: center;
}

.nav-item {
    font-family: "Geometria";
    text-transform: uppercase;
    line-height: 20px;
    font-weight: 700;
}

.basket {
    position: relative;
    margin: 0;
    display: flex;
    align-items: center;
}

.basket-heading {
    margin: 0;
    margin-bottom: 2px;
    color: #9a9a9a;
    font-family: "TT Norms Pro";
    font-weight: 400;
    line-height: 14px;
    font-size: 12px;
}

.basket-sum {
    margin: 0;
    font-family: "TT Norms Pro";
    font-weight: 500;
    font-size: 14px;
    line-height: 21px;
}

#basket {
    margin-right: 15px;
}

#ellipse {
    position: absolute;
    top: 5px;
    left: 20px;
}

/* стили для выпадающего списка */
.nav-menu__list {
    display: flex;
    flex-direction: column;
    position: absolute;
    background: #ffffff;
    height: 200px;
    padding: 20px;
    z-index: 100;
    box-shadow: 5px 5px 2px 1px #9a9a9a;
    border-top-right-radius: 30px;
    border-bottom-right-radius: 30px;
}

.nav-menu__item {
    font-family: "Geometria";
    text-transform: uppercase;
    line-height: 20px;
    font-weight: 700;
}
</style>