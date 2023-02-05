<template>
    <div class="profile">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-6">
                    <div class="d-flex text-start">
                        <div class="flex-shrink-0">
                            <img src="../assets/poto.jpg" class="mr-3 user-pic" alt="...">
                        </div>
                        <div class="flex-grow-1 ms-3">
                            <h5>{{ firstName }} Evan {{ lastName }}</h5>
                           <p>{{ bio }}</p> 
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
  
  import 'bootstrap/dist/css/bootstrap.css'

  export default {
    name: 'ProfileView',
    data: function(){
        return{
            firstName: 'Anggito',
            lastName : 'Kusumo',
            bio: 'So, above that is a name which is their parents are portugies and javanese. that was awesome right?'      
        }
    },
    components: {
      // HelloWorld
    }
  }
  </script>

  <style scoped>
    .user-pic{
        border-radius: 200%;
        height: 120px;
        widows: 120px;
    }
</style>