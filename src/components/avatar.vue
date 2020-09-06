<template>
  <figure class="avatar">
      <img :src="src" :alt="alt" :width="size" :height="size" />
  </figure>
</template>

<script>
export default {
  name: "Avatar",
  props: {
    src: {
      type: String,
      default:
        'https://instagram.fyei1-1.fna.fbcdn.net/v/t51.2885-19/s150x150/96419061_251445949559965_4554525574290210816_n.jpg?_nc_ht=instagram.fyei1-1.fna.fbcdn.net&_nc_ohc=qZPGsH-yWGkAX_30oJ-&oh=a205d3a047a6dde2d54c8bb623b716ff&oe=5F7FA220'
    },
    alt: {
      type:String
    },
    size: {
      type: Number
    }
  }

}
</script>

<style scoped>
.avatar{
  display: inline-flex;
  padding: 2px;
  border-radius: 999px;
  background: linear-gradient(90deg,
  rgba(184,63,140,1) 0%,
  rgba(237,158,90,1) 100%);

  img{
    border-radius: inherit;
    border: 2px solid white;

  }
}
</style>