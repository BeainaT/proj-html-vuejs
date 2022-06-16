<template>
  <div class="course_card">
        <img :src="course.img" :alt="course.typo">
        <div class="details px-2">
            <h5>{{course.title}}</h5>
            <span>{{course.type}}</span>
            <hr>
            <div class="icons mb-3 d-flex justify-content-around">
                <small><i class="fa-solid fa-signal color"></i>{{course.level}}</small>
                <small><i class="fa-solid fa-list-ul color"></i>{{course.total}}</small>
                <small><i class="fa-regular fa-clock color"></i>{{course.time}}</small>
            </div>
        </div>
  </div>
</template>

<script>
export default {
    name: 'CourseCard',
    props: {
        course: Object
    },
}
</script>

<style lang="scss" scoped>
    .course_card {
        background-color: var(--secondary_color);
        font-family: var(--typo_sans_serif);
        border: 1px solid var(--card_line);
        img {
            width: 100%;
            min-height: 12.5rem;
            margin-bottom: 1rem;
        }
        h5 {
            font-family: var(--typo_serif);
            margin: 1rem 0;
        }

        span,
        hr {
            color: var(--card_secondary);
        }
        .color {
            color: var(--primary_color);
            margin: 0 .3125rem;

        }
    }

</style>