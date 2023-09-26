<template>
  <div id="app">
    <task v-bind:tasks="tasks"></task>
  </div>
</template>

<script>
import Task from "./components/Task";

export default {
  name: "App",
  components: {
    Task,
  },
  data() {
    return {
      tasks: [
        {
          id: 1,
          title: "Go Shopping",
          completed: true,
        },
        {
          id: 2,
          title: "Watch Naruto",
          completed: true,
        },
        {
          id: 3,
          title: "Learn Python",
          completed: false,
        },
        {
          id: 4,
          title: "Learn Guitar",
          completed: false,
        },
        {
          id: 5,
          title: "Send Email to Hr",
          completed: false,
        },
      ],
    };
  },
};
</script>