<template>
  <div id="app">
    <the-header title="The Avengers"></the-header>
    <employee-content :employeeList="employeeList"></employee-content>
  </div>
</template>

<script>
import EmployeeContent from './components/employee/EmployeeContent.vue';
import TheHeader from './components/layout/TheHeader.vue';

export default {
  components: {
    EmployeeContent,
    TheHeader,
  },
  data() {
    return {
      employeeList: [
        {
          id: 1,
          name: 'John Doe',
          title: 'Software Engineer',
          link: 'https://example.com/john-doe',
        },
        {
          id: 2,
          name: 'Jane Smith',
          title: 'Product Manager',
          link: 'https://example.com/jane-smith',
        },
        {
          id: 3,
          name: 'Alice Johnson',
          title: 'Data Scientist',
          link: 'https://example.com/alice-johnson',
        },
        {
          id: 4,
          name: 'Bob Williams',
          title: 'UI/UX Designer',
          link: 'https://example.com/bob-williams',
        },
      ],
    };
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>
