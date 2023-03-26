<template>
    <div class="row">
        <div class="col" v-for="item in items">
            <div class="box">
                <div class="w-100 h-100">
                    <div class="box-img" :style="{ 'background-image': 'url(' + item.imgUrl + ')' }"></div>
                </div>
                <div class="fw-bolder text-center"> {{ item.itemName }} </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue'

const items = ref([
    {
        imgUrl: "/src/assets/img/item.png",
        itemName: "吊扇"
    }, {
        imgUrl: "/src/assets/img/item.png",
        itemName: "洗手槽"
    }, {
        imgUrl: "/src/assets/img/item.png",
        itemName: "電壁爐"
    }, {
        imgUrl: "/src/assets/img/item.png",
        itemName: "冰淇淋機"
    }, {
        imgUrl: "/src/assets/img/item.png",
        itemName: "床包"
    }
])
</script>

<style scoped>
.box {
    width: 5rem;
    height: 5rem;
    margin: 0 auto;
    float: none;
}

.box-img {
    max-width: 100%;
    height: 100%;
    background-size: 100% 100%;
}

</style>