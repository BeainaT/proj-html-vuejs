<template>
  <div class="course_card p-0" :class="{special_badge : course.isSpecial}">
        <div class="hover_box">
            <img :src="course.img" :alt="course.typo">
            <span>$59</span>

        </div>
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
        width: calc(100% / 4);
        position: relative;
        &.special_badge::after {
            content:"SPECIAL";
            background-color: var(--special_badge);
            color: var(--secondary_color);
            border-radius: .1875rem;
            font-weight: 400;
            font-family: var(--typo_serif);
            font-size: 0.75rem;
            padding: .25rem;
            position: absolute;
            top: .625rem;
            right: .625rem;

        }
        &:hover img {
            filter: brightness(0.7);
        }
        &:hover .hover_box span {
            display: block;
        }
        .hover_box {
            position: relative;
            span {
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
                color: var(--secondary_color);
                font-size: 2rem;
                font-weight: bold;
                display: none;
            }
        }
        img {
            width: 100%;
            min-height: 12.5rem;
            margin-bottom: 1rem;
            position:relative;
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