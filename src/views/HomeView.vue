<template>
  <div class="home">

    <div class="container">
      <div class="row header mb-3 p-3">
        <div class="col-lg-12">
          <h1 class="m-0">What Should I Do Today?</h1>
        </div>
      </div>
      <div class="row content">
        <div class="col-lg-12">
          <div class="homework">

            <div v-for="myTask in task" v-bind:key="myTask.id" class="task">
              
              <ItemTask v-bind:myTask="myTask" />

            </div>

          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import ItemTask from '@/components/ItemTask.vue';

export default {
  name: 'HomeView',
  data: function() {
    return {
      task: [
        {
          id :1,
          nama: "Cleaning Toilet",
          isDone: false
        },
        {
          id :2,
          nama: "Cleaning Kitchen",
          isDone: false
        },
        {
          id :3,
          nama: "Cleaning Bed",
          isDone: false
        },
        {
          id :4,
          nama: "Cleaning Desk",
          isDone: false
        },
      ]
    };
  },
  components: {
    ItemTask
  }
}
</script>

<style scoped>

.header{
  background-color: #a3f;
}

</style>