//v-for berfungsi untuk perunglangan berdasrkan key

<template>
  <div id="app">
   <div class="container">
      <div class="row header mb-5 p-3">
          <div class="col-lg-12">
              <h2>What I do Today ?</h2>
          </div>
      </div>
      <div class="row content">
          <div class="col col-lg-12">
    <div class="pekerjaan-rumah">
      <div class="row">
       <div v-for="tugasSaya in tugas" v-bind:key="tugasSaya.id" class="mb-4 tugas col-lg-12 text-start">
       <input class="form-check-input" onclick="" type="checkbox" value="" id="flexCheckDefault">
          <label class="form-check-label item " v-bind:class="{'item-completed':tugasSaya.isDone}" for="flexCheckDefault">{{  tugasSaya.namaTugas}}</label>
  
      </div>
      </div>
    </div>
      </div>
      </div>
   </div>
  </div>
</template>

//v-bind:class itu membuat statement kondisi kalau is.done di javascript done maka warna hijau yang muncul

<script>

import 'bootstrap/dist/css/bootstrap.css'


export default{
  name: 'AboutView',
  data: function() {
    return{
    tugas: [
      {
        id: 1,
        namaTugas: "Membersihkan Toilet",
        isDone: false
      },
      {
        id: 2,
        namaTugas: "Menjadi Anak Yang Berguna Bagi Kedua Orang Tua",
        isDone: true
      }, 
      {
        id: 3,
        namaTugas: "Menjadi Anak Yang Bisa Membantu Kedua Orang Tua",
        isDone: false
      },
       {
        id: 4,
        namaTugas: "Selalu Jaga Kesehatan",
        isDone: false
      }
    ]
    }; 
  },
  components: {
   
  }
};

</script>


<style>
.header{
  background: #1abc9c;
}

.header h2 {
  margin: 0;
}

.tugas .item{
  font-size: 20px;
}

.item-completed{
  color: #1abc9c;
}

</style>