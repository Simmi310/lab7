<template>
    <h3>รายชื่อวิชาทั้งหมด</h3>
    <hr />
    <table>
      <tr>
        <th>รหัสวิชา</th>
        <th>ชื่อวิชา</th>
      </tr>
  
      <tr v-for="(course, index) in courses" :key="index">
        <td style="text-align: left">{{ course.course_id }}</td>
        <td style="text-align: left">
          {{ course.course_name }}
        </td>
      </tr>
    </table>
</template>
  