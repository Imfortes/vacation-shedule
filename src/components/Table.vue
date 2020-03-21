<template>
    <table class="table" style="width: 90vw;">
        <thead>
            <tr>
                <th v-for="(label, index) in labels" :key="index">
                    {{ label.title }}
                </th>
            </tr>
        </thead>
        <tbody>
            <tr v-for="person in persons" :key="person.id">
                <td class="name"><img src="../assets/photo-2.png" alt="">{{person.name}}</td>
                <td class="days">{{person.days}}</td>
                <td>
                    <div :class="[person.jan === 0 ? 'cell' : 'holidays']" v-on:mouseover="mouseOver">
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                    </div>
                </td>
                <td>
                    <div :class="[person.feb === 0 ? 'cell' : 'holidays']" v-on:mouseover="mouseOver">
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                    </div>
                </td>
                <td>
                    <div :class="[person.march === 0 ? 'cell' : 'holidays']" v-on:mouseover="mouseOver">
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                    </div>
                </td>
                <td>
                    <div :class="[person.apr === 0 ? 'cell' : 'holidays']" v-on:mouseover="mouseOver">
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                    </div>
                </td>
                <td>
                    <div :class="[person.may === 0 ? 'cell' : 'holidays']" v-on:mouseover="mouseOver">
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                    </div>
                </td>
                <td>
                    <div :class="[person.jun === 0 ? 'cell' : 'holidays']" v-on:mouseover="mouseOver">
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                    </div>
                </td>
                <td>
                    <div :class="[person.jul === 0 ? 'cell' : 'holidays']" v-on:mouseover="mouseOver">
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                    </div>
                </td>
                <td>
                    <div :class="[person.aug === 0 ? 'cell' : 'holidays']" v-on:mouseover="mouseOver">
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                    </div>
                </td>
                <td>
                    <div :class="[person.sep === 0 ? 'cell' : 'holidays']" v-on:mouseover="mouseOver">
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                    </div>
                </td>
                <td>
                    <div :class="[person.oct === 0 ? 'cell' : 'holidays']" v-on:mouseover="mouseOver">
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                    </div>
                </td>
                <td>
                    <div :class="[person.nov === 0 ? 'cell' : 'holidays']" v-on:mouseover="mouseOver">
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                    </div>
                </td>
                <td>
                    <div :class="[person.dec === 0 ? 'cell' : 'holidays']" v-on:mouseover="mouseOver">
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                        <div class="cell-item"></div>
                    </div>
                </td>
            </tr>
        </tbody>
    </table>
</template>

<script>
export default {
    data() {
        return{
            labels: [
                {id: 0, title: 'Фамилия, Имя'},
                {id: 1, title: 'дней'},
                {id: 2, title: 'Янв'},
                {id: 3, title: 'Фев'},
                {id: 4, title: 'Мар'},
                {id: 5, title: 'Апр'},
                {id: 6, title: 'Май'},
                {id: 7, title: 'Июн'},
                {id: 8, title: 'Июл'},
                {id: 9, title: 'Авг'},
                {id: 10, title: 'Сен'},
                {id: 11, title: 'Окт'},
                {id: 12, title: 'Ноя'},
                {id: 13, title: 'Дек'},
            ],
            persons: [
                {id: 0, img: 'photo.png', name: 'Иван Иванов', days: '14/28', jan: 0, feb: 0, march: 0, apr: 14, may: 0, jun: 0, jul: 0, aug: 0, sep: 0, oct: 0, nov: 0, dec: 0},
                {id: 1, img: 'photo-2.png', name: 'Катерина Иванова', days: '14/28', jan: 0, feb: 0, march: 0, apr: 0, may: 0, jun: 0, jul: 0, aug: 14, sep: 0, oct: 0, nov: 0, dec: 0},
                {id: 2, img: 'photo.png', name: 'Петр Иванов', days: '14/28', jan: 0, feb: 0, march: 3, apr: 1, may: 4, jun: 4, jul: 0, aug: 0, sep: 2, oct: 0, nov: 0, dec: 0},
                {id: 3, img: 'photo-2.png', name: 'Юлия Иванова', days: '14/28', jan: 0, feb: 0, march: 7, apr: 0, may: 0, jun: 0, jul: 0, aug: 0, sep: 0, oct: 0, nov: 0, dec: 7},
                {id: 4, img: 'photo.png', name: 'Василий Иванов', days: '14/28', jan: 0, feb: 0, march: 0, apr: 2, may: 12, jun: 0, jul: 0, aug: 0, sep: 0, oct: 0, nov: 0, dec: 0}
            ],
            methods: {
                mouseOver: function (event) {
                    if  (event.target.classList.contains('holidays')){
                        console.log('console:' + event);
                    }
                }
            }
        }
    }
}
</script>

<style scoped>
    .table{
        margin: 0 auto !important;
        background: #f7f7f7;
        border: 0;
        border-collapse: collapse;
        border-spacing: 0;
    }
    thead{
        background: #f7f7f7;
    }
    th{
        padding: 10px 5px;
    }
    tbody{
        background: #ffffff;
    }
    td{
        background-color: #fff;
        border: none;
        padding: 10px 5px;
    }
    .days{
        text-align: center;
    }
    .cell,
    .holidays,
    .name{
        height: 100%;
        margin: 0 !important;
        padding: 0;
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
    }
    .name{
        justify-content: flex-start;
        padding: 10px 0 5px 10px;
    }
    .name img{
        margin-right: 10px;
    }
    .holidays .cell-item{
        background: #1ebeb4;
    }
    .cell-item{
        width: 8px;
        height: 16px;
        background: #eaf9ff;
        margin: 0 1px 0 1px;
    }
</style>