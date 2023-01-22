<template>
    <div class="w-full border-t-2 border-slate-300 text-center">
        <a :href="`${dailyUILink}`">
            <h2 class="text-2xl pt-2">{{ title }}</h2>
            <p class="text-left"> {{ date }} </p>
        </a>
    </div>
    <slot></slot>

</template>
<script>

export default {
  props: {
    title: String,
    date: String,
    dailyUILink: String,
    }
}

</script>