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
  <div>
    <img style=" padding: 18px;" class="m-auto"
         src="../assets/images/iRadio/screen1.webp" alt="" width="300" height="300">
    <img style=" padding: 18px;" class="m-auto"
         src="../assets/images/iRadio/screen2.webp" alt="" width="300" height="300">
    <div>
      <div>
        <h1>iRadio</h1>
        <h1>An app for listen radios all round world</h1>
        <h1>It's free with no ads</h1>
      </div>
      <br><br><br>
      <span>
        <h1>Android</h1>
        <form method="get"
              action='https://ps-1314295485.cos.ap-shanghai.myqcloud.com/beast_Official_5.6.9_build00177.apk'>
          <button
            btn m-3 text-sm
          >
            {{ t('button.Download') }}
          </button>
        </form>
      </span>
      <span>
        <h1>iOS</h1>
        <form method="get"
        >
          <button
            btn m-3 text-sm
          >
            {{ t('button.ComingSoon') }}
          </button>
        </form>
      </span>
    </div>
  </div>
</template>
