<script setup>

</script>
<template>
    <div class="flex flex-col w-96 bg-gray-100 mx-auto rounded-lg p-8 space-y-2">
        <h1 class="text-4xl mb-8">Login Form</h1>
        <div class="flex   sm:flex-row  flex-col ">
            <a class="p-2 hover:text-white    bg-gradient-to-l from-pink-500 to-purple-500 bg-green-300 rounded-md text-white border flex-auto  content-center "
                href="#">Login</a>
            <a class="p-2 rounded-md text-black border flex-auto  bg-white  content-center   " href="#">Signup</a>
        </div>
        <input type="text" name="myemail" value="" placeholder="Email"  class=" border p-3 rounded-md   h-12">
        <input type="text" name="" value="" id="" placeholder="Password" class=" border p-3 rounded-md   h-12">
        <a href="#" class="text-left text-pink-400" >Forgot Password?</a>
        <button class="bg-gradient-to-l from-pink-500 to-purple-500 text-white hover:text-white text-2xl">Login</button>
        <span>Not a member <a href="#">Signup now </a> </span>


    </div>
</template>

<style scoped></style>
