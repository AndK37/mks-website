<template>
    <div>
        <card-item img_path="categories/image1.png" name="Стекло"></card-item>
        <card-item img_path="categories/image2.png" name="Мягкая кровля и гидроизоляция"></card-item>
        <card-item img_path="categories/image3.png" name="Битумы"></card-item>
        <card-item img_path="categories/image4.png" name="Стеклопакеты"></card-item>
        <card-item img_path="categories/image5.png" name="Электроды"></card-item>
        <card-item img_path="categories/image6.png" name="Круги отрезные, зачистные"></card-item>

        <card-item img_path="categories/image7.png" name="Парафин"></card-item>
        <card-item img_path="categories/image8.png" name="Мастики, Праймер, Грунтовки, Клей и Герметики"></card-item>
        <card-item img_path="categories/image9.png" name="Утеплители, пароизоляция, пленка"></card-item>
        <card-item img_path="categories/image10.png" name="Стеклоблок"></card-item>
        <card-item img_path="categories/image11.png" name="Гвозди"></card-item>
        <card-item img_path="categories/image12.png" name="Алмазный инструмент"></card-item>
    </div>

</template>

<script>
import CardItem from "../components/CardItem.vue"

export default {
    components: {
        "card-item": CardItem,
    }
}
</script>

<style scoped>

div {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    max-width: 1100px;
    margin-left: auto;
    margin-right: auto;
}

</style>