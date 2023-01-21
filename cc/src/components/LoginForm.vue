<template>
<div class="login-form w-64 h-96 border-2 border-green-500">
  <div class="sign-tab flex flex-row justify-around ">
    <div class="cursor-pointer hover:bg-slate-200 hover:text-green-300 w-full text-center p-2">Sign In</div>
    <div class="cursor-pointer hover:bg-slate-200 hover:text-green-300 w-full text-center p-2">Sign Up</div>
  </div>
  <div class="form-controls flex flex-col justify-center">
    <div class="flex flex-row mx-6 border-b-2 border-green-300 mt-10 p-1 content-center">
      <input class="mr-2 w-40 p-0.5" type="text" placeholder="Username">
      <img class="w-4" src="/public/user-solid.svg" alt="user icon">
    </div>
    <div class="flex flex-row mx-6 border-b-2 border-green-300 mt-5 p-1">
      <input class="mr-2 w-40 p-0.5" type="password" placeholder="Password">
      <img class="w-4" src="/public/lock-solid.svg" alt="lock icon">
    </div>
    <div class="flex text-xs mt-10 gap-1 mx-2 justify-around">
      <div class="flex">
        <input class="mr-1 accent-green-300" type="checkbox">
        <p class="text-green-300">Remember me?</p> 
      </div>
      <a class="underline" href="#">Forgot password</a>
    </div>
    <div class="flex justify-center mt-3 h-10">
      <button class="bg-[#f0ad58] w-52">Log In</button>

    </div>
    <div class="flex flex-col text-center mt-3">
      <div class="">or</div>
      <div class="flex flex-row bg-blue-600 w-52 h-10 mx-auto mt-1 justify-around content-center">
          <img src="/public/fb.png" alt="Facebook" class="w-6 h-6 mt-1.5">
        <button>Log in with Facebook</button>
      </div>
    </div>
  </div>

</div>
</template>