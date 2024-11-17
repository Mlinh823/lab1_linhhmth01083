<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <!-- <div><a>{{ username }}</a><a>{{ password }}</a></div> -->
  <div>
    <a v-html="username"></a>
  </div>
  <div>
    <button v-on:click="changeUserName">Change username</button> 
  </div>

  <div>
    <button v-bind:class="btnClass" v-on:click="changebtnClass">Dữ liệu v-Bind</button>
  </div>

  <div>
    <button v-on:click="changeimgLink">Đổi ảnh</button>
      <img v-bind:src="imgLink">
  </div>

  
</template>

<script>
export default {
  data() {
    return {
      username: 'user01',
      password: '1',
      email: 'a@example.com',
      btnClass: 'btn btn-success',
      imgLink:'https://toigingiuvedep.vn/wp-content/uploads/2022/04/anh-hai-huoc.jpg'
    }
  },
  methods:{
      changeUserName()
      {
        this.username = 'New username'
      },
      changebtnClass(){
        this.btnClass = 'btn btn-danger'
      },
      changeimgLink(){
        this.imgLink = 'https://s.meta.com.vn/img/thumb.ashx/Data/image/2021/11/05/hinh-anh-meme-hai-huoc-anh-che-meme-16.jpgs'
      }
    }
}
</script>

<style scoped>
</style>