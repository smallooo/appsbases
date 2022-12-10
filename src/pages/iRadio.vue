<script setup lang="ts">
const props = defineProps<{ name: string }>()
const router = useRouter()
const user = useUserStore()
const { t } = useI18n()

watchEffect(() => {
  user.setNewName(props.name)
})
</script>

<template>
  <div>
    <img class="m-auto"
         src="../assets/images/collection01/naruto_02.png" alt="" width="300" height="300">
    <h1>This is iRadio</h1>
    <h1>This is iRadio</h1>
  </div>
</template>
