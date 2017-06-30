<template>
<div>   
    <app-stock v-for="sotck in stocks"></app-stock>
    </div>
</template>

<script>
    import Stock from './Stock.vue';

export default {
    data(){
        return{
            stocks:[
                { id:1, name: 'CARLITOS', edad: 24 },
                { id:2, name: 'YORSH', edad: 25 },
                { id:3, name: 'ALAN', edad: 20 },
                { id:4, name: 'ISAIAS', edad: 23 }
            ]
        }
    },
    components: {
        appStock: Stock
    }
}
</script>
