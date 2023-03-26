<template>
    <footer class="bk-color-basic container-fluid text-light">
        <div class="row p-3">
            <div class="col-12 fs-3 fw-bold">
                得利購HOME
            </div>
            <div class="col-2 mt-3">
                <div class="fs-6 fw-bold mb-3">客戶服務</div>
                <div class="fs-6">預約體驗</div>
                <div class="fs-6">常見問題</div>
            </div>
            <div class="col-4 mt-3">
                <div>
                    <div class="fs-6 fw-bold mb-3">聯絡我們</div>
                    <div class="fs-6">台北市中山區德惠街60號1樓
                        <br>
                        (02)2585-6161 ｜平日 09:00 - 18:30
                        <br>
                        <a class="text-light" href="https://support@directgo.tw" target="_blank">support@directgo.tw</a>
                    </div>
                </div>
            </div>
            <div class="col-6 mt-3">
                <div>
                    <div class="fs-6 fw-bold mb-3">歡迎加入, 更認識我們</div>
                    <a class="" href="/" target="">
                        <i class="bi bi-facebook text-light fs-4"></i>
                    </a>
                    <a class="ms-4" href="/" target="">
                        <i class="bi bi-line text-light fs-4"></i>
                    </a>
                    <a class="ms-4" href="/" target="">
                        <i class="bi bi-youtube text-light fs-4"></i>
                    </a>
                </div>
            </div>
            <div class="col-12 position-relative mt-5" style="height: 3.5rem;">
                <div class="position-absolute top-50 end-0 translate-middle-y">
                    <BlackBtn btn-text="預約體驗" :style="{width: '6.4rem'}"/>
                </div>
            </div>
            <div class="col-12">
                <p class="" style="font-size: 15px;">
                    © directgo home 2022
                </p>
            </div>
        </div>
    </footer>
</template>

<script setup>
import BlackBtn from './object/BlackBtn.vue'
</script>

<style scoped>

</style>
