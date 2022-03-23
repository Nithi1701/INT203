<script setup>
    import { ref } from 'vue';

    const students = ref([
        {studentId: 111, studentName: 'chan'},
        {studentId: 222, studentName: 'o'},
        {studentId: 333, studentName: 'cha'}
    ])
</script>
 
<template>
    <div>
        <ul>
            <li v-for="student in students" :key="student.id">
                Student Name:
                <router-link
                :to="{
                    name: 'StudentItem',
                    params: { studentId: student.studentId }
                }">
                {{ student.studentName }}
                </router-link>
            </li>
        </ul>
    </div>
</template>
 
<style>

</style>