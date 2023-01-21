<script>
export default {
  data() {
  	return {
      // true - login
      // false - sign up
	    signingType: true
  	}
	}
}
</script>
<template>
<div class="login-form w-64 min-h-96 border-2 border-green-500 pb-12">
  <div class="sign-tab flex flex-row justify-around ">
    <div @click="signingType = true" class="cursor-pointer hover:bg-slate-200 hover:text-green-300 w-full text-center p-2">
      Sign In
    </div>
    <div @click="signingType = false" class="cursor-pointer hover:bg-slate-200 hover:text-green-300 w-full text-center p-2">
      Sign Up
    </div>
  </div>
  
  <div class="form-controls flex flex-col justify-center gap-4">
    <div class="flex flex-row mx-6 border-b-2 border-green-300 mt-5 p-1 content-center">
      <input class="rounded mr-2 w-40 p-0.5" type="text" placeholder="Username">
      <img class="w-4 invert" src="/public/user-solid.svg" alt="user icon">
    </div>

    <div v-if="!signingType" class="flex flex-row mx-6 border-b-2 border-green-300 p-1 content-center">
      <input class="rounded mr-2 w-40 p-0.5" type="text" placeholder="Email">
      <img class="w-4 invert" src="/public/envelope-regular.svg" alt="email icon">
    </div>

    <div class="flex flex-row mx-6 border-b-2 border-green-300 p-1">
      <input class="rounded mr-2 w-40 p-0.5" type="password" placeholder="Password">
      <img class="w-4 invert" src="/public/lock-solid.svg" alt="lock icon">
    </div>

    <div v-if="signingType" class="flex text-xs mt-2 gap-1 mx-2 justify-around">
      <div class="flex">
        <input class="mr-1 accent-green-300" type="checkbox">
        <p class="text-green-300">Remember me?</p> 
      </div>
      <a class="underline" href="#">Forgot password</a>
    </div>
    <div v-else class="flex text-sm mt-2 mx-2 justify-center gap-4">
      <div class="flex">
        <input class="mr-1 accent-green-300" type="checkbox">
        <p class="text-green-300">Male</p> 
      </div>
      <div class="flex">
        <input class="mr-1 accent-green-300" checked type="checkbox">
        <p class="text-green-300">Female</p> 
      </div>
    </div>

    <div class="flex justify-center mt-3 h-10">
      <button class="bg-orange-400 active:bg-orange-300 w-52">
        {{ signingType ? "LOG IN" : "SIGN UP" }}
      </button>

    </div>
    <div class="flex flex-col text-center">
      <div class="flex row content-center justify-center align-middle">
        <div class="w-8 h-0 border-[0.5px] border-green-500 mt-3"></div>
        <div class="mx-3">or</div>
        <div class="w-8 h-0 border-[0.5px] border-green-500 mt-3"></div>
      </div>
      <div class="flex flex-row bg-blue-600 active:bg-blue-500 w-52 h-10 mx-auto mt-2 justify-around content-center">
          <img src="/public/fb.png" alt="Facebook" class="w-6 h-6 mt-1.5">
        <button>
          {{`${signingType ? "Log In" : "Sign Up"} with Facebook`}}
        </button>
      </div>
    </div>
  </div>

</div>
</template>