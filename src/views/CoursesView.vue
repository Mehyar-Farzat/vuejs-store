<template>
  <h2>Courses Page</h2>
  <div>
    <CourseList/>
  </div>

  <div>
    <CourseFilter/>
  </div>

</template>

<script>

  import CourseList from '@/components/CoursList.vue'
  import CourseFilter from '@/components/CourseFilter.vue'
  
  export default {
    name: 'CoursesPage',
    components:{
      CourseList,
      CourseFilter
    }
  }
</script>