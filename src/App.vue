<template>
  <HelloWorld msg="Welcome"/>
  <CarouselComponent/>
  <NavbarComponent/>
  
  <div v-for="book in books" :key="book.title">
    <p>
      {{book.title}}
    </p>

</div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import CarouselComponent from './components/CarouselComponent.vue'
import NavbarComponent from './components/NavbarComponent.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    CarouselComponent,
    NavbarComponent
  },
  data(){
      return {
        good:'Good Evening',
        books:{
          book1:{
            title:'my title',
            author:'abdoo',
            stars:5
          },
          book2:{
            title:'your title',
            author:'abdoo',
            stars:2
          }
        }
      };
  }

}
</script>

<style>

</style>
