<template>
    <div>
        <app-stock v-for="(stock, index) in stocks" :key="index"></app-stock>
    </div>
</template>
<script>
import Stock from "./Stock.vue"
export default {
    data() {
        return {
            stocks : [
                {id: 1, name: "Microsoft", price: 110},
                {id: 2, name: "Apple", price: 300},
                {id: 3, name: "Amazon", price: 240},
                {id: 4, name: "Facebook", price: 180},
            ]
        }
    },
    components: {
        appStock: Stock,
    }
}
</script>
