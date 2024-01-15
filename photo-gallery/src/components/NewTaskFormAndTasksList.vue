<template>
  <ion-page>
    <NewTaskForm />
    <TaskList />
  </ion-page>
</template>

<script>

  import NewTaskForm from '../components/NewTaskForm.vue'
  import TasksList from '../components/TasksList.vue'

  export default {
    name: 'App',
    components: {
      NewTaskForm,
      TasksList,
    }
  }
</script>

<style lang="scss" scoped>

</style>