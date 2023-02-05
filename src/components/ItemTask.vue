<template>
    <div>
        <div class="form-check d-inline-block mb-2">

<input class="form-check-input" onclick="" type="checkbox" v-bind:id="myTask.id">
<label class="form-check-label" v-bind:class="{'text-success':myTask.isDone}" v-bind:for="myTask.id">
  {{ myTask.id }}. {{ myTask.nama }}
</label>

</div>
    </div>
</template>

<script>

export default{
    name: "ItemTask",
    props: ["myTask"]
}


</script>

<style scoped>



</style>