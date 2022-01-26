<script setup>
// array
  const courses = ['INT203', 'INT204', 'INT205', 'INT206']
// obj
  const myAccount = {
    accountId:1234,
    accounName:'Nithi',
    blance: 99999
  }
// Ex
  const courses2 = [
    { courseId: 'INT201', courseName: 'Client I', credit: 2 },
    { courseId: 'INT202', courseName: 'Client II', credit: 2 },
    { courseId: 'INT210', courseName: 'Architecture and Deployment', credit: 3 }
  ]
</script>
 
<template>
<!-- array -->
  <ul>
    <li v-for="(course, index) in courses" :key="index">{{ index }} - {{ course }}</li>
  </ul>
<!-- obj -->
  <ul>
    <li v-for="(value, propKey, index) in myAccount" :key="index">
      {{ index }} - {{ propKey }}: {{ value }}
    </li>
  </ul>
<!-- Ex -->
 <ul>
    <li v-for="(course, index) in courses2" :key="index">
      {{ course.courseId }} : {{ course.credit }} : {{ course.courseName }}
    </li>
  </ul>
</template>
 
<style>

</style>