<template>
  <div class="home">
    <CustomText tag="h1">Profile</CustomText>
    <CustomText tag="p">Lorem Ipsum, dizgi ve baskı endüstrisinde kullanılan mıgır metinlerdir. Lorem Ipsum, adı bilinmeyen bir matbaacının bir hurufat numune kitabı oluşturmak üzere bir yazı galerisini alarak karıştırdığı 1500'lerden beri endüstri standardı sahte metinler olarak kullanılmıştır. Beşyüz yıl boyunca varlığını</CustomText>
    <div id="nav">
      <router-link to="/profile">Post</router-link> | |
      <router-link to="/profile/igtv">IGTV</router-link> |
      <router-link to="/profile/save">Save</router-link> |
      <router-link to="/profile/tag">Tag</router-link>
    </div>

    <router-view />
  </div>
</template>

<script>
import CustomText from '@/components/CustomText'

export default {
  name: "Profile",
  components: {
  CustomText
  }
};
</script>

<style scoped></style>
