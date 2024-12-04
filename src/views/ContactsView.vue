<template>
    <div class="contacts">
        <table>
            <tr>
                <td style="text-align: end;">Адрес:</td>
                <td>г. Екатеринбург, район Уктус, база «Уктус» </td>
            </tr>
            <tr>
                <td></td>
                <td>ул. Походная, 81, Литер «И» оф. 33, 3-й этаж. Склад № 20А</td>
            </tr>
            <tr>
                <td style="text-align: end;">Отдел продаж:</td>
                <td>тел. (343) 213-84-84 , +79089219942 </td>
            </tr>
            <tr>
                <td></td>
                <td>Директор Яковлев Виталий Игоревич</td>
            </tr>
            <tr>
                <td style="text-align: end;">E-mail:</td>
                <td><span>2466085@mail.ru</span></td>
            </tr>
            <tr>
                <td style="text-align: end;">Время работы:</td>
                <td>c 9 - 00 до 16 - 00 без перерыва</td>
            </tr>
            <tr>
                <td></td>
                <td>Суббота, Воскресение - выходной</td>
            </tr>
            <tr>
                <td style="text-align: end;">Реквизиты:</td>
                <td>ОГРН 1106674021739, ИНН/КПП 6674368391/667401001</td>
            </tr>
            <tr>
                <td></td>
                <td>ОКПО 90051685 </td>
            </tr>
            <tr>
                <td></td>
                <td>р/с 40702810322560001405 ФАКБ «АБСОЛЮТ БАНК»</td>
            </tr>
            <tr>
                <td></td>
                <td>(ПАО) в г. Екатеринбурге, к/с 30101810800000000921</td>
            </tr>
            <tr>
                <td></td>
                <td>БИК 046577921</td>
            </tr>
        </table>
        <img src="../assets/img/image4.png" alt="">
    </div>
</template>

<script>

</script>

<style scoped>
* {
    font-family: 'Arial';
    font-style: normal;
    font-weight: 400;
    font-size: 24px;
    line-height: 29px;
    color: #000000;
}

.contacts {
    margin-left: auto;
    margin-right: auto;
    max-width: 1000px;
}

span {
    text-decoration: underline;
}

tr:nth-child(odd) {
    background-color: #d4d4d4;
}

tr:nth-child(even) {
    background-color: #e5e5e5;
}

td {
    padding: 10px;
}

table {
    margin-left: auto;
    margin-right: auto;
    width: 100%;
}

img {
    width: 100%;
    display: block;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 70px;
    padding-top: 20px;
}

@media (max-width: 750px) {
  * {
    font-family: 'Arial';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 19px;
    text-align: center;
    color: #000000;
  }
  img {
    display: none;
  }
}
</style>
