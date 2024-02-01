<template>
  
  <div class="container py-5">
    <div class="row">
      <div class="col-lg-3">
        <CourseFilter/>
      </div>
      <div class="col-lg-9">
        <CourseList/>
      </div>
    </div>
  </div>
  
</template>

<script>

  import CourseList from '@/components/CoursList.vue'
  import CourseFilter from '@/components/CourseFilter.vue'
  import { courses } from '../tem-data'
  
  export default {
    name: 'CoursesPage',
    components:{
      CourseList,
      CourseFilter
    }
  }
</script>