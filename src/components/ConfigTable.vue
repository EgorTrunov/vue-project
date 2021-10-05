<template>
    <div class="container">
        <h2 class="title__question">Какой формы должен быть стол?</h2>
        <ul class="question__list">
            <li class="question__item form__table">
                <div class="question__block">
                    <img class="form__table-img" src="@/assets/img/form_rectangle.jpg" alt="Стол прямоугольной формы" width="350" height="232">
                    <h3 class="form__table-title">Прямоугольным</h3>
                    <p class="form__table-text">Подоберите все необходимое для оформления завершенного, гармоничного, стильного и уютного интерьера своей квартиры или дома в одном месте.</p>
                </div>
                <div class="question__block">
                    <img class="form__table-img" src="@/assets/img/form_square.jpg" alt="Стол квадратной формы" width="350" height="232">
                    <h3 class="form__table-title">Квадратным</h3>
                    <p class="form__table-text">Подоберите все необходимое для оформления завершенного, гармоничного, стильного и уютного интерьера своей квартиры или дома в одном месте.</p>                    
                </div>
                <div class="question__block">
                    <img class="form__table-img" src="@/assets/img/form_circle.jpg" alt="Стол круглой формы" width="350" height="232">
                    <h3 class="form__table-title">Круглым</h3>
                    <p class="form__table-text">Подоберите все необходимое для оформления завершенного, гармоничного, стильного и уютного интерьера своей квартиры или дома в одном месте.</p>
                </div>
            </li>
        </ul>
    </div>
</template>


<script>
export default {
    name: 'ConfigTable'
    
}
</script>

<style scoped>
.title__question {
    font-weight: 600;
    font-size: 18px;
    line-height: 26px;
    text-align: center;
    margin: 15px 0 70px;
}

.question__item {
    display: flex;
    justify-content: space-between;
}

.question__block {
    width: 350px;
    display: flex;
    flex-direction: column;
}

.form__table-title {
    font-size: 24px;
    line-height: 24px;
    margin: 0;
    margin-top: 40px;
}

.form__table-text {
    font-weight: 300;
    font-size: 14px;
    line-height: 24px;
    margin-top: 40px;
    margin-bottom: 10px;
}

.form__table-img {
    filter: grayscale(1);
    transition: 1s;
    cursor: pointer;
}

   .form__table-img:hover {
    filter: grayscale(0);
}
</style>