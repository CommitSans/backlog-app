<template>
  <div>
    <h2>Add game</h2>
    <form @submit.prevent='createNewTask'>
      <div>
        <label for="newTaskDescription">Game description</label>
        <input type="text" placeholder='add game description' required v-model="newTask.description">
        <ion-button type="submit">Add game</ion-button>
      </div>
    </form>
  </div>
</template>

<script>
  import { reactive } from 'vue'
  // import { db } from '../firebase'

  export default {
    setup() {
      const newTask = reactive ({
        creationTime: null,
        description: '',
        completed: false,
      })
      // const taskCollection = db.collection('tasks')

      const createNewTask = () => {
        taskCollection.add({
          ...newTask,
          creationTime: Date.now()
        })

        newTask.description = ''
      }

      return {
        newTask,
        createNewTask,
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>