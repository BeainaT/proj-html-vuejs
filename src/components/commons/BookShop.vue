<template>
  <div class="container pt-5">
    <div class="row justify-content-center align-items-center">
        <div class="col-5">
            <h2>Get my exclusive investing Book just for $19.50</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Numquam quam, delectus odio sed voluptatum nostrum minus similique culpa?</p>
            <a href="#"><img class="amazon_btn" src="../../assets/img/amazon.png" alt="amazon link"></a>
        </div>
        <div class="col-5">
            <img class="img_book" src="../../assets/img/book.png" alt="book company">
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'BookShop'
}
</script>

<style lang="scss" scoped>
    h2 {
        color: var(--primary_color);
        font-family: var(--typo_sans_serif);
        font-weight: 500;
    }
    p {
        font-family: var(--typo_italic);
        font-size: 1.25rem;
        margin: 1.5rem 0;
    }
    .img_book {
        width: 100%;
    }
    .amazon_btn {
        max-width: 10rem;
    }
</style>