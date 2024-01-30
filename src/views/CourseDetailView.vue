<template>
  <div class="container">
    <div class="row my-5">
      <div class="col-lg-6">
        <img :src="course.image" class="img-fluid" alt="">
      </div>
      <div class="col-lg-6">
        <h2>{{ course.name }}</h2>
        <h4>{{ course.category }}</h4>
        <p>{{ course.prise }}$</p>
        <button class="btn btn-secondary">Enroll</button>
      </div>
    </div>
  </div>
</template>

<script>
import { course, courses } from '../tem-data'
  export default {
    name: 'CourseDetailPage',
    data(){
      return {
        course: courses.find(course => course.id == this.$route.params.course_id)
      }
    }
  }
</script>