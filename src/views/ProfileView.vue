<template>
<div class="profile">
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-12">
              <div class="d-flex text-start">
                <div class="flex-shrink-4 ">
                 <img src="../assets/riski.jpg" class="mr-3 user-pic">
                </div>
                    <div class="mt-0">
                    <h5>{{ firstName }} {{ lastName }}</h5>
                    <p>{{ description }}</p>
                     </div>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
// kita import dulu boostrap
import 'bootstrap/dist/css/bootstrap.css'


export default {
  name: 'ProfileView',
  data: function(){
    return {
         firstName: 'Rizki',
         lastName: 'Mahendra',
         description: 'Perkenalkan Nama Saya Rizki Mahendra Saya Berasal Dari Kota Pekanbaru'
    }
  },
  components: {
    // ProfileView
  }
}
</script>

<style scoped>
.user-pic {
    border-radius: 200%;
    height:120px;
    width:120px;
}
</style>