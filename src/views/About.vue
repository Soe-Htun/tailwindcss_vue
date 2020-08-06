<template>
    <div>
        <ul class="flex inline-block justify-between">
            <li class="ml-2">
                <a class="text-black-500 text-xl focus:text-blue-500">Active</a>
            </li>
            <li >
                <a class="text-black-500 text-xl focus:text-blue-500">Link</a>
            </li>
            <li >
                <a class="text-black-500 text-xl focus:text-blue-500" >Link</a>
            </li>
            <li >
                <a class="text-gray-500 text-xl cursor-not-allowed" >Disabled</a>
            </li>
            <li >
                <a class="float-right mr-2 text-xl focus:text-blue-500 cursor-pointer" @click="logout()">logout</a>
            </li>
        </ul>
        <br>
        <h2 class="font-bold text-5xl mt-10">Hello, welcome from About page</h2>

        <div class="flex items-center bg-gray-200 h-24">
            <div class="flex-1 text-gray-700 text-center bg-gray-400 px-4 py-2 m-2">1</div>
            <div class="flex-1 text-gray-700 text-center bg-gray-400 px-4 py-2 m-2">2</div>
            <div class="flex-1 text-gray-700 text-center bg-gray-400 px-4 py-2 m-2">3</div>
        </div>
    </div>
</template>

<script>
export default {
    name:'app',
    data() {
        return {
            
        }
    },
    methods:{
        logout(){
            this.$router.replace('/')
        }
    }
}
</script>>