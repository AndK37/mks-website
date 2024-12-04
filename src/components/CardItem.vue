<template>
    <div class="card">
        <div class="card-item">
            <img :src="img_path" alt="">
            <div class="shadow">
                <span>{{ name }}</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        img_path: String, 
        name: String
    }
}
</script>

<style scoped>
img {
    width: 100%;
    z-index: 5;
}
.card {
    cursor: pointer;
    margin: 10px;
}
.card-item {
    position: relative;
    width: 490px;
    height: 270px;
}

.shadow {
    width: 490px;
    height: 270px;
    position: absolute;
    top: 0px;
    left: 0px;
    box-shadow: 0px -150px 80px -100px rgba(0, 0, 0, 1) inset;
    z-index: 10;
}

span {
    font-family: 'Arial';
    font-style: normal;
    font-weight: 400;
    font-size: 24px;
    line-height: 29px;
    color: #FFFFFF;
    position: absolute;
    bottom: 15px;
    left: 30px
}

@media (max-width: 576px) {
    .card-item {
    position: relative;
    width: 100%;
    height: 195px;
}
img {
    width: 100%;
    height: 195px;
    z-index: 5;
}
.shadow {
    width: 100%;
    height: 195px;
    position: absolute;
    top: 0px;
    left: 0px;
    box-shadow: 0px -150px 80px -100px rgba(0, 0, 0, 1) inset;
    z-index: 10;
}
}
</style>