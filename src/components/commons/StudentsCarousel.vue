<template>
    <div class="row align-items-center">
        <div class="col-2">
            <i class="fa-solid fa-arrow-left-long arr_font"></i>
        </div>
        <div class="col-8">
            <div class="row justify-content-center align-items-center">
                <div class="col-2 px-1">
                    <img src="../../assets/img/1-100x100.jpg" alt="smiling guy">
                </div>
                <div class="col-3 px-2 mx-1">
                    <img src="../../assets/img/2-100x100.jpg" alt="smiling guy">
                </div>
                <div class="col-2 px-1">
                    <img src="../../assets/img/4-100x100.jpg" alt="smiling guy">
                </div>
            </div>
        </div>
        <div class="col-2">
            <i class="fa-solid fa-arrow-right-long arr_font"></i>
        </div>
    </div>
</template>

<script>
export default {
    name: 'StudentsCarousel'
}
</script>

<style lang="scss" scoped>
.arr_font {
    font-size: 1.5625rem;
}
img {
    border-radius: 100%;
    width: 100%;
}

</style>