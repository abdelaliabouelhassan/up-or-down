<template>
<NuxtLayout :name="layout">
  <NuxtPage />
</NuxtLayout >
</template>


<script setup>
 const layout = ref('main')
 const route = useRoute()
 const { localePath } = useRouter()
 const setLayout = (name) => {
   layout.value = name
 }

 const checkLayout = (name) => {
    if (name === 'index') {
      setLayout('main')
    } else  if (name === 'up-or-down') {
      setLayout('updown')
    } 
 }



 //set layout based on route path
  watch(() => route.name, () => {
    checkLayout(route.name)
  })

  onMounted(() => {
    checkLayout(route.name)
    console.log(route.name)
  })


 
</script>