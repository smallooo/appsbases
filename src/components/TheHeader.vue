<script setup lang="ts">
const { t, availableLocales, locale } = useI18n()

const toggleLocales = () => {
  // change to some real logic
  const locales = availableLocales
  locale.value = locales[(locales.indexOf(locale.value) + 1) % locales.length]
}
</script>

<template>
  <nav text-xl mt-6>
    <RouterLink class="icon-btn mx-2" to="/iRadio" :title="t('button.about')">
      <img class="icon-btn mx-2" style="border-radius: 10%;"
           src="../assets/images/iRadio/icon.webp" alt="" width="100" height="100">
      <br>
      <h3>iRadio</h3>
    </RouterLink>
    <RouterLink class="icon-btn mx-2" to="/PetStation" :title="t('button.about')">
      <img class="icon-btn mx-2"
           src="../assets/images/collection01/naruto_02.png" alt="" width="100" height="100">
      <br>
      <h3>PetStation</h3>
    </RouterLink>
<!--    <RouterLink class="icon-btn mx-2" to="/resume" :title="t('button.about')">-->
<!--      <img class="icon-btn mx-2"-->
<!--           src="../assets/images/collection01/naruto_02.png" alt="" width="100" height="100">-->
<!--      <h3>故诗配图</h3>-->
<!--    </RouterLink>-->
<!--    <RouterLink class="icon-btn mx-2" to="/resume" :title="t('button.about')">-->
<!--      <img class="icon-btn mx-2"-->
<!--           src="../assets/images/collection01/naruto_02.png" alt="" width="100" height="100">-->
<!--      <h3>千千静听</h3>-->
<!--    </RouterLink>-->
<!--    <RouterLink class="icon-btn mx-2" to="/resume" :title="t('button.about')">-->
<!--      <img class="icon-btn mx-2"-->
<!--           src="../assets/images/collection01/naruto_02.png" alt="" width="100" height="100">-->
<!--      <h3>iRadio</h3>-->
<!--    </RouterLink>-->
<!--    <RouterLink class="icon-btn mx-2" to="/resume" :title="t('button.about')">-->
<!--      <img class="icon-btn mx-2"-->
<!--           src="../assets/images/collection01/naruto_02.png" alt="" width="100" height="100">-->
<!--      <h3>iRadio</h3>-->
<!--    </RouterLink>-->
<!--    <RouterLink class="icon-btn mx-2" to="/resume" :title="t('button.about')">-->
<!--      <img class="icon-btn mx-2"-->
<!--           src="../assets/images/collection01/naruto_02.png" alt="" width="100" height="100">-->
<!--      <h3>iRadio</h3>-->
<!--    </RouterLink>-->
<!--    <RouterLink class="icon-btn mx-2" to="/resume" :title="t('button.about')">-->
<!--      <img class="icon-btn mx-2"-->
<!--           src="../assets/images/collection01/naruto_02.png" alt="" width="100" height="100">-->
<!--      <h3>iRadio</h3>-->
<!--    </RouterLink>-->
  </nav>
</template>
