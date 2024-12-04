<template>
  <div class="home">
    <p>Компания “МетКровСтрой” реализует строительные и отделочные материалы в Екатеринбурге. Работать в сфере
      снабжения наши специалисты начали еще в 90-х годах прошлого века. Огромный опыт сотрудников, успешные и
      долговременные связи с поставщиками, позволяют нам предлагать покупателю товары по недорогим ценам.</p>
    <img src="../assets/img/image1.png" alt="">
    <p>Подберем под заказ все, что в наших силах: стройматериалы, оборудование, инстумент, крепеж, лакокраску,
      металлопрокат, спецодежду, хозяйственные принадлежности, сантехнику, электронику, электрику и
      т.д. Скомплектуем
      товары на нашем складе, упакуем, подготовим у отгрузке. Можем принять ваш товар от продавцов на временное
      хранение, и также отгрузить по требованию.</p>
    <img src="../assets/img/image2.png" alt="">
    <p>Также обращаем Ваше внимание на наш широкий ассортимент продукции, в котором представлены такие популярные
      товары
      для общестроительных работ, как <span>битум</span>, <span>электроды</span>, <span>мастики</span>,
      <span>наполавляемая кровля</span> и отделки - <span>стеклоблоки</span> для
      обустройства ванных комнат, комнатных перегородок, стен, и т.д. На сегодняшний день мы
      являемся единственными поставщиками с наличием на складе цветных и бесцветных стеклоблоков.
    </p>
    <img src="../assets/img/image3.png" alt="">
  </div>

</template>

<script>
// @ is an alias to /src
export default {

}
</script>

<style scoped>
.home {
  max-width: 1000px;
  margin-left: auto;
  margin-right: auto;
}

p {
  font-family: 'Arial';
  font-style: normal;
  font-weight: 400;
  font-size: 24px;
  line-height: 29px;
  text-align: center;
  color: #000000;
}

img {
  width: 100%;
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 70px;
}

span {
  text-decoration: underline;
}

@media (max-width: 750px) {
  p {
    font-family: 'Arial';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 19px;
    text-align: center;
    color: #000000;
  }


}
</style>
