<template>
    <div class="container">
        <div class="best">
            <p class="gray">ЛУЧШИЕ В СВОЕМ ДЕЛЕ</p>
            <h2 class="title best-title">Что позволило нам за 5 лет стать производителем №1 в мире эксклюзивной мебели из редких пород дерева?</h2>
        </div>
        <div class="about">
            <dl class="about__list">
                <div class="img__container">
                    <img class="about__img" src="@/assets/img/сertificate.png" alt="" width="475" height="334">
                </div>
                <div class="about__text">
                    <dt class="about__title">Полностью сертифицированная продукция</dt>
                    <dd class="about__explanation">Подоберите все необходимое для оформления завершенного, гармоничного, стильного и уютного интерьера своей квартиры или дома в одном месте.</dd>
                </div>
                <div class="about__text">
                    <dt class="about__title">Конкурентные цены при высоком качестве и широком ассортименте</dt>
                    <dd class="about__explanation">Подоберите все необходимое для оформления завершенного, гармоничного, стильного и уютного интерьера своей квартиры или дома в одном месте.</dd>
                    <button class="button about__btn">В каталог</button>
                </div>
                <img class="about__img img__2" src="@/assets/img/model_1.png" alt="" width="540" height="682">
                <img class="about__img img__3" src="@/assets/img/model_2.png" alt="475" width="471">
                <div class="about__text">
                    <dt class="about__title about__title-left">Постоянный контроль этапов работ перед заказчиком</dt>
                    <dd class="about__explanation">Подоберите все необходимое для оформления завершенного, гармоничного, стильного и уютного интерьера своей квартиры или дома в одном месте.</dd>
                </div>
                <div class="about__text">
                    <dt class="about__title about__title-left">Изготавливаем мебель любой сложности в течение указанного срока в договоре</dt>
                    <dd class="about__explanation">Подоберите все необходимое для оформления завершенного, гармоничного, стильного и уютного интерьера своей квартиры или дома в одном месте.</dd>
                </div>
                <img class="about__img img__4" src="@/assets/img/blanks.png" alt="" width="540" height="285">
                <img class="about__img img__5" src="@/assets/img/work-time.png" alt="" width="475" height="348">
                <div class="about__text">
                    <dt class="about__title">Первоклассные специалисты готовы ответить на любые ваши вопросы</dt>
                    <dd class="about__explanation">Подоберите все необходимое для оформления завершенного, гармоничного, стильного и уютного интерьера своей квартиры или дома в одном месте.</dd>
                </div>
            </dl>
        </div>
    </div>
</template>

<script>
export default {
    name: 'About'
}
</script>

<style scoped>
.best {
    margin-top: 65px;
    text-align: center;
}

.best p {
    margin: 0;
    text-transform: uppercase;
    margin-bottom: 15px;
}

.best-title {
    padding: 0 135px;
    margin-bottom: 70px;
}

.about__list {
    display: grid;
    grid-template-columns: 475px 540px;
    column-gap: 95px;
    grid-template-rows: 395px 468px 103px 110px 361px 346px 358px;
}

.about__title {
    font-weight: bold;
    font-size: 24px;
    line-height: 34px;
    margin: 0;
    margin-top: 60px;
    margin-bottom: 30px;
    max-width: 340px;
}

.about__text:nth-of-type(3) {
    grid-row: 5 / 6;
    grid-column: 2 / 3;
}

.about__text:nth-of-type(4) {
    grid-row: 6 / 7;
    grid-column: 1 / 2;
}

.about__text:last-of-type {
    grid-row: 7 / 8;
    grid-column: 2 / 3;
}

.about__title-left {
    margin-left: auto;
    margin-right: -40px;
}

.about__explanation {
    font-weight: 300;
    font-size: 14px;
    line-height: 24px;
    margin-left: auto;
    margin-right: 50px;
    max-width: 350px;
}

.about__btn {
    margin: 90px auto 50px 70px;
}

.about {
    background: url("../assets/img/decor.svg"); 
}

.img__2 {
    grid-row: 2 / 5;
    grid-column: 2 / 3;
}

.img__3 {
    grid-row: 4 / 6;
    grid-column: 1 / 2;
}

.img__4 {
    grid-row: 6 / 7;
    grid-column: 2 / 3;
}

.img__5 {
    grid-row: 7 / 8;
    grid-column: 1 / 2;
}
</style>