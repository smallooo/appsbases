<script setup lang="ts">
const props = defineProps<{ name: string }>()
const router = useRouter()
const user = useUserStore()
const { t } = useI18n()

const iOS = () => {

}

watchEffect(() => {
  user.setNewName(props.name)
})
</script>

<template>
  <br><br><br>
  <img class="icon-btn mx-2" style="border-radius: 3%;"
       src="../assets/images/ComingSoon.jpg" alt="" width="300" height="300">
  <br><br>
  <h1> Coming soon</h1>
</template>
