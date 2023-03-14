<template>
  <!-- <GreetmeCard name="Stephen" />
  <GreetmeCard name="Micheal" />
  <GreetmeCard name="Maggie"  />
  <GreetmeCard :name="name"  :hobby="hobby" />
  <ArticleBlog title="Article Title" :likes="50" :isPublished="true" /> -->
  <button @click="showPopup=true">Show Popup</button>
  <PopupWindow v-show="showPopup" @close="Closepopup" />
</template>

<script>
// import GreetmeCard from './components/GreetmeCard.vue'
// import ArticleBlog from './components/ArticleBlog.vue'
import PopupWindow from './components/PopupWindow.vue'

export default {
  name: 'App',
  components: {
    // GreetmeCard,
    // ArticleBlog,
    PopupWindow,
  },
  data(){
    return{
      //  name:'Stephen',
      //  hobby:'coding',
       showPopup:false,
    }
  },
  methods:{
      Closepopup(name){
          this.showPopup=false
          console.log('name',name)
      }
    }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
