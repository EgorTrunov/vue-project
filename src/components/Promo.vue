<template>
    <div class="container">
        <div class="promo">
            <div class="column-text">
                <h1 class="promo-title">Авторская <span>мебель</span></h1>
                <h2 class="Rosanthie-text">Design</h2>
                <h3 class="promo-title-text">из слэбов редких пород древесины</h3>
                <p class="promo-text">Подоберите все необходимое для оформления завершенного, гармоничного, стильного и уютного интерьера своей квартиры или дома в одном месте.</p>
            </div>
            <div class="column-img">
                <img class="promo-img" src="@/assets/img/promo-table.png" alt="Стол из редкой древесины с 'рекой' посередине" width="650" height="600">
                <div class="video">
                    <img src="@/assets/img/video.jpg" alt="Картинка видео, но только пока">
                    <p>Посмотрите на производство WOODCRAFTSTUDIO</p>    
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Promo'    
}

</script>

<style scoped>

.promo {
    display: grid;
    grid-template-columns: 2fr 1fr;
}

.promo-title {
    font-family: 'Kudryashev Display';
    font-size: 150px;
    line-height: 150px;
    font-weight: 400;
    margin-top: 50px; 
}

span {
    display: block;
    margin-left: -100px;
    text-align: center;
}

.Rosanthie-text {
    left: 390px;
    top: 270px;
    font-weight: 400;
}

.promo-title-text {
    font-size: 20px;
    line-height: 26px;
    text-align: center;
    margin: -45px 0 50px -170px;
}

.promo-text {
    width: 450px;
    color: #A3A3A3;
}

.promo-img {
    position: absolute;
    left: 680px;
}

.video {
    position: absolute;
    width: 300px;
    height: 225px;
    left: 1000px;
    top: 490px;
    text-align: end;
}

.video p {
    font-family: 'Geometria';
    font-style: normal;
    font-weight: normal;
    font-size: 14px;
    line-height: 24px;
}

</style>