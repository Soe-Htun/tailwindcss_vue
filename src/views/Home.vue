<template>
<div>
  <div class="bg-gray-200 py-4">
    <span class="block text-gray-700 bg-gray-400 px-4 py-2">1</span>
    <span class="block text-gray-700 text-center bg-gray-400 px-4 py-2 mt-2">2</span>
    <span class="block text-gray-700 text-center bg-gray-400 px-4 py-2 mt-2">3</span>
  </div>

  <div class="bg-gray-200">
    <div class="inline-block text-gray-700 text-center bg-gray-400 px-4 py-2 m-2">1</div>
    <div class="inline-block text-gray-700 text-center bg-gray-400 px-4 py-2 m-2">2</div>
    <div class="inline-block text-gray-700 text-center bg-gray-400 px-4 py-2 m-2">3</div>
  </div><br>
  

  <input type="text" v-model="name" placeholder="Enter name" class="border border-gray-500 focus:border-blue-400 px-6 py-2 rounded-full outline-none mt-20" /><br><br>
  <input v-model="password" placeholder="Enter password" class=" border border-gray-500  focus:border-blue-400 py-2 px-6 rounded-full outline-none"> <br><br>
  <button class=" bg-blue-500 text-gray-200 px-6 py-2 rounded-full focus:bg-blue-700" @click="login()">Login</button>
  <button class=" bg-blue-500 text-gray-200 px-6 py-2 ml-5 rounded-full" @click="clear()">Clear</button><br><br>

</div>
 
</template>

<script>
export default {
  name: 'Nav',
  data() {
    return {
      name:'',
      password:''
    }
  },
  methods:{
    login(){
      this.$router.replace({name:"about"})
    },
    clear(){
      this.name ='';
      this.password =''
    }
  }
}
</script>


