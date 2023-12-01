<template>
    <div class="w-screen h-screen bg-violet-400 flex justify-center py-20">
        <div class="w-1/2 py-20 px-20 bg-white h-auto rounded-lg">
            <h1 class="text-2xl font-thin mb-8">Edible Project</h1>
            <h2 class="text-3xl font-semibold mb-3">Login</h2>
            <p class="text-thi mb-20">Please login using your credentials</p>
            <h5 class="text-sm font-semibold mb-3">Username</h5>
            <input class="p-3 w-full border border-black rounded mb-5" v-model="username">
            <h5 class="text-sm font-semibold mb-3">Password</h5>
            <input class="p-3 w-full border border-black rounded mb-10" v-model="password">
            <button class="w-full p-3 bg-zinc-900 text-white text-center rounded" @click="submitLoginForm">
                Login
            </button>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            username: 'username1',
            password: 'test1'
        }
    },
    methods: {
        submitLoginForm: function() {
            navigateTo('/homepage')
        }
    }
}
</script>
