<template>
  <div class="container">
    <div class="row">
      <div class="col-lg-6">
        <img :src="course.image" alt="">
      </div>
      <div class="col-lg-6">
        <h2>{{ course.name }}</h2>
        <h4>{{ course.category }}</h4>
        <p>{{ course.prise }}$</p>
        <button>Enroll</button>
      </div>
    </div>
  </div>
</template>

<script>
import { course } from '../tem-data'
  export default {
    name: 'CourseDetailPage'
  }
</script>