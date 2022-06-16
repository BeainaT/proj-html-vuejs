<template>
    <section class="founder_wishes container pb-4"> 
        <div class="row justify-content-center">
            <div class="col-4">
                <h2>Hey there, my name is John Doe. I'm the founder of the Brain Academy.</h2>
                <div class="sign_box py-4">
                    <img src="../../assets/img/sign.jpg" alt="founder sign">
                </div>
            </div>
            <div class="col-5">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Id voluptate omnis ad? Cupiditate ducimus harum provident quis eum? Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur laboriosam necessitatibus dolore molestias in rem quis ea porro ipsa. Est tempore in voluptatibus, laudantium quas quam deserunt debitis similique expedita. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Autem ipsa harum veniam soluta hic, quia ut eaque maxime suscipit quos nostrum cumque. Assumenda aspernatur qui beatae illum magnam soluta placeat!</p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FounderWishes'
}
</script>

<style lang="scss" scoped>
    .founder_wishes {
        position: relative;
        > .row {
            gap: 1.875rem;
        }
        .sign_box {
            text-align: center;
        }
        top: -3.125rem
    }
</style>