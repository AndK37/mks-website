<template>
    <div class="header">
        <div v-if="windowW > 750" class="top">
            <div class="title">
                <span class="bold">МКС</span>
                <span>Предприятие</span>
            </div>
            <button class="btn">Позвонить</button>
            <span>+7 (343) 213-84-84</span>
        </div>
        <div v-else class="top">
            <div class="title">
                <span class="bold">МКС</span>
                <span>Предприятие</span>
            </div>

            <div class="call">
                <button class="btn">Позвонить</button>
                <span>+7 (343) 213-84-84</span>
            </div>
            <svg class="svg3" width="30" height="30" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
                <circle cx="18" cy="12" r="11" stroke="black" stroke-width="2" />
                <line x1="1.25671" y1="29.331" x2="10.2567" y2="19.331" stroke="black" stroke-width="2" />
            </svg>

        </div>

        <div class="nav">
            <svg class="svg1" width="32" height="30" viewBox="0 0 32 30" fill="none" xmlns="http://www.w3.org/2000/svg">
                <line x1="11" y1="30" x2="11" stroke="black" stroke-width="2" />
                <line y1="29" x2="32" y2="29" stroke="black" stroke-width="2" />
                <line y1="6" x2="32" y2="6" stroke="black" stroke-width="2" />
                <line x1="25" y1="7" x2="25" y2="20" stroke="black" stroke-width="2" />
                <rect x="22" y="19" width="6" height="6" stroke="black" stroke-width="2" />
                <line x1="10.206" y1="2.02145" x2="29.206" y2="6.02145" stroke="black" stroke-width="2" />
                <line x1="11.4061" y1="1.91381" x2="2.40614" y2="5.91381" stroke="black" stroke-width="2" />
            </svg>
            <RouterLink to="/">Главная</RouterLink>
            <RouterLink to="/catalog">Каталог</RouterLink>
            <RouterLink to="/about">Стеклоблоки</RouterLink>
            <RouterLink to="/about">Услуги</RouterLink>
            <RouterLink to="/contacts">Контакты</RouterLink>

            <svg class="svg2" width="30" height="30" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
                <circle cx="18" cy="12" r="11" stroke="black" stroke-width="2" />
                <line x1="1.25671" y1="29.331" x2="10.2567" y2="19.331" stroke="black" stroke-width="2" />
            </svg>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            windowW: window.innerWidth
        }
    },
    mounted() {
        this.$nextTick(() => {
            window.addEventListener('resize', this.onResize);
        })
    },
    methods: {
        onResize() {
            this.windowW = window.innerWidth
        }
    }
}
</script>

<style scoped>
* {
    font-family: "Arial";
    font-style: normal;
    font-weight: 400;
    font-size: 24px;
    line-height: 29px;
}

.bold {
    font-family: 'Arial';
    font-style: normal;
    font-weight: 700;
    font-size: 36px;
    line-height: 44px;
}

.header {
    display: flex;
    flex-direction: column;
    max-width: 1000px;

    margin-left: auto;
    margin-right: auto;
    margin-top: 20px;
    margin-bottom: 20px;
}

.btn {
    border: none;
    border-radius: 50px;
    background-color: #e13b3b;
    padding: 10px 20px 10px 20px;
    color: #fff;
    cursor: pointer;
    margin-bottom: 10px;
}

.title {
    display: flex;
    flex-direction: column;
    align-items: start;
}

.top {
    padding-left: 8%;
    padding-right: 8%;
    padding-bottom: 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.call {
    display: flex;
    flex-direction: column;
}

.nav a.router-link-exact-active {
    color: #000;
    text-decoration: none;
    font-weight: 700;
}

.nav a {
    color: #000;
    text-decoration: none;
}

@media (max-width: 750px) {
    * {
        font-family: "Arial";
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 19px;
    }

    .bold {
        font-family: 'Arial';
        font-style: normal;
        font-weight: 700;
        font-size: 32px;
        line-height: 39px;
    }

    .header {
        display: flex;
        flex-direction: column;
        margin-left: 0;
        margin-right: 0;
    }

    .top {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding-left: 0%;
        padding-right: 0%;
    }

    .svg1,
    .svg2 {
        display: none;
    }
}
</style>
