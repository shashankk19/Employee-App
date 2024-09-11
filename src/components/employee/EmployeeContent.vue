<template>
  <ul>
    <employee-item
      v-for="employee in employeeList"
      :key="employee.id"
      :name="employee.name"
      :title="employee.title"
      :link="employee.link"
    >
    </employee-item>
  </ul>
</template>

<script>
import EmployeeItem from './EmployeeItem.vue';

export default {
  components: {
    EmployeeItem,
  },
  props: ['employeeList'],
  data() {},
};
</script>

<style scoped>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>
