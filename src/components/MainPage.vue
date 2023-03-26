<template>
    <body>
        <div class="container-fluid g-0">
            <div class="row g-0">
                <div class="col-sm-6">
                    <div class="ratio ratio-1x1">
                        <video class="object-fit-fill" controls autoplay loop muted>
                            <source src="../assets/video/Pexels Videos 1721286.mp4" type="video/mp4">
                        </video>
                    </div>
                </div>
                <div class="col-sm-6">
                    <div class="w-100 ratio ratio-1x1">
                        <div class="display-area-div-img text-light">
                            <div class="position-absolute top-0 end-0 p-3">
                                <span class="me-2 fw-bold" name="spaceBtn" value="taipei"
                                    v-on:mouseover="chgImg('/src/assets/img/1.png', 'taipei')">台北館</span>
                                <span class="me-2">|</span>
                                <span class="me-2" name="spaceBtn" value="taichung"
                                    v-on:mouseover="chgImg('/src/assets/img/2.png', 'taichung')">台中館</span>
                            </div>
                            <div class="position-absolute top-50 start-50 translate-middle ">
                                <div class="text-center fs-1 fw-bold">VIP展空間</div>
                                <div class="text-center fs-5">私人VIP專業顧問介紹</div>
                                <div class="black-btn text-center mt-3">
                                    <BlackBtn btn-text="預約體驗" :style="{ width: '6.4rem' }" />
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row p-5 g-0">
                <div class="col">
                    <HomePageCarousel />
                </div>
            </div>
            <div class="row g-0">
                <div class="col pt-4 ps-4 pe-4">
                    <div class="ratio ratio-16x9">
                        <div class="display-bad-div-img text-light">
                            <div class="position-absolute top-50 end-0 translate-middle-y"
                                style="width: 22rem; padding-right: 5rem;">
                                <div class="fs-3 fw-bold lh-1">帶你享受<br>從未有過的沈靜</div>
                                <div class="mt-2" style="font-size: 0.8rem;">
                                    現省數十萬，送席夢思黑標枕。席夢思床墊符合人體工學設計，精準釋放壓力、紓解疲勞，讓您享受全然放鬆健康舒適的睡眠！</div>
                                <div class="black-btn text-center mt-3">
                                    <BlackBtn btn-text="了解更多" :style="{ width: '17rem' }" />
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row g-0">
                <div class="col pt-4 ps-4 pe-4">
                    <div class="ratio ratio-16x9">
                        <div class="display-kichen-div-img text-light">
                            <div class="position-absolute top-50 start-0 translate-middle-y"
                                style="width: 22rem; padding-left: 5rem;">
                                <div class="fs-3 fw-bold lh-1">迎接體面的廚房生活</div>
                                <div class="mt-2" style="font-size: 0.8rem;">
                                    雙手不必觸碰廚餘，廚房清潔再次升級，發揮卓越的廚房功效，為你省去一輩子輕掃廚餘的時間！</div>
                                <div class="black-btn text-center mt-3">
                                    <BlackBtn btn-text="了解更多" :style="{ width: '17rem' }" />
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row g-0">
                <div class="col-sm-6">
                    <div class="ratio ratio-1x1">
                        <div class="display-rh-div-img text-light">
                        </div>
                    </div>
                </div>
                <div class="col-sm-6">
                    <div class="w-100 ratio ratio-1x1">
                        <div class="">
                            <div class="position-absolute top-50 start-50 translate-middle w-75">
                                <div class="fs-1 fw-bold">RH × 得利購</div>
                                <div class="fs-6">美國Restoration Hardware 家具(簡稱RH)受到高端客戶推崇，融合古典建築與現代設計，是奢華夢幻逸品家具品牌。</div>
                                <div class="black-btn mt-3">
                                    <BlackBtn btn-text="了解更多" :style="{ width: '17rem' }" />
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row g-0">
                <div class="col-12 row g-0">
                    <div class="col-6 fw-bold fs-5 p-4">
                        精選品單
                    </div>
                    <div class="col-6">
                        <div class="position-absolute end-0 fs-5 fw-bolder p-4">
                            <lookAllBtn />
                        </div>
                    </div>
                </div>
                <div class="col-12 p-3">
                    <CommodityInCarousel />
                </div>
            </div>
            <div class="row g-0">
                <div class="col-12 row g-0">
                    <div class="col-6 fw-bold fs-5 p-4">
                        熱門文章
                    </div>
                    <div class="col-6">
                        <div class="position-absolute end-0 fs-5 fw-bolder p-4">
                            <lookAllBtn />
                        </div>
                    </div>
                </div>
                <div class="col-12 row p-3">
                    <div class="col-6 popular-articles-area-div-img">
                        <div class="w-100 ratio ratio-16x9"></div>
                    </div>
                    <div class="col-6W popular-articles-area-div-img">
                        <div class="w-100 ratio ratio-16x9"></div>
                    </div>
                </div>
            </div>
        </div>
    </body>
</template>

<script setup>
import BlackBtn from './object/BlackBtn.vue'
import HomePageCarousel from './object/HomePageCarousel.vue'
import CommodityInCarousel from './object/CommodityInCarousel.vue'
import lookAllBtn from './object/lookAllBtn.vue'

function chgImg(imgUrl, value) {
    document.querySelector(".display-area-div-img").style = "background-image: url('" + imgUrl + "')"
    document.querySelector("span[name='spaceBtn']").classList.remove('fw-bold')
    document.querySelector("span[value='" + value + "']").classList.add('fw-bold')
}
</script>


<style scoped>
.display-area-div-img {
    background-image: url("/src/assets/img/1.png");
}

.display-bad-div-img {
    background-image: url("/src/assets/img/bad.png");
}

.display-kichen-div-img {
    background-image: url("/src/assets/img/kichen.png");
}

.display-rh-div-img {
    background-image: url("/src/assets/img/RH.png");
}

.popular-articles-area-div-img {
    background-image: url("/src/assets/img/popularArticles.png");
}

.display-area-div-img,
.display-bad-div-img,
.display-kichen-div-img,
.display-rh-div-img,
.popular-articles-area-div-img {
    background-size: 100% 100%;
    background-position: center center;
    transition: linear 0.5s;
}

.display-area-div-img:has(.black-btn:hover),
.display-bad-div-img:has(.black-btn:hover),
.display-kichen-div-img:has(.black-btn:hover),
.display-rh-div-img:hover,
.popular-articles-area-div-img:hover  {
    background-size: 150% 150%;
}
</style>