<template>
  <section>
    <div class="container py-5">
      <h2>new courses</h2>
      <div class="row justify-content-center pb-5">
        <CourseCard v-for="(course, i) in courses" :key="i" :course="course" />
      </div>
      <button>load more</button>
    </div>
  </section>
</template>

<script>
import CourseCard from '../commons/CourseCard.vue'
export default {
    name: 'CourseSection',
    components: {
      CourseCard
    },
    data() {
      return {
        courses: [
          {
            img: require("../../assets/img/photo-1496307042754-b4aa456c4a2d-370x200.jpeg"),
            title: "How to be a DJ? Make Electronic Music",
            type: "Electronic",
            level: "Advanced",
            total: "8 Lectures",
            time : "6 hours",
            isSpecial: true
          },
          {
            img: require("../../assets/img/12345-1-370x200.png"),
            title: "Nvidia and UE4 Technologies Practice",
            type: "Nvidia",
            level: "Advanced",
            total: "8 Lectures",
            time : "6 hours",
            isSpecial: true

          },
          {
            img: require("../../assets/img/photo-1491897554428-130a60dd4757-370x200.jpeg"),
            title: "Fashion Photography from professional",
            type: "Fashion",
            level: "Advanced",
            total: "6 Lectures",
            time : "6 hours",
            isSpecial: true
          },
          {
            img: require("../../assets/img/photo-1416339134316-0e91dc9ded92-370x200.jpeg"),
            title: "Design Instruments for Communication",
            type: "Communication",
            level: "Intermediate",
            total: "6 Lectures",
            time : "6 hours",
            isSpecial: false
          },
          {
            img: require("../../assets/img/cathryn-lavery-67852-unsplash-370x200.jpg"),
            title: "Make your Concept Right and Beautiful",
            type: "Art",
            level: "Intermediate",
            total: "6 Lectures",
            time : "6 hours",
            isSpecial: false
          },
          {
            img: require("../../assets/img/photo-1475452779376-caebfb988090-370x200.jpeg"),
            title: "Road Bike Manual or How to Be a Champion",
            type: "Bicycling",
            level: "Beginner",
            total: "6 Lectures",
            time : "6 hours",
            isSpecial: false
          },
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
  section {
    background-color: var(--bg_light);
    text-align: center;
    h2 {
      text-transform: capitalize;
      font-weight: bold;
      font-size: 2.5rem;
      margin-bottom: 2rem;
    }
    .row {
      gap: 1.25rem
    }
    button {
      background-color: var(--primary_color);
      font-weight: bold;
      padding: .625rem 1.25rem;
    }

  }

</style>