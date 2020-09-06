<template>
  <div class="home">

    <div class="timeline">
      <h1>Home</h1>

      <br />
      <br />
      <br />
      <br />

       <Post />

      <br />
      <br />
      <br />
      <br />
      <br />
      <br />
    </div>


    <div class="sidebar">
      <p>Lorem Ipsum, dizgi ve baskı endüstrisinde
        kullanılan mıgır metinlerdir. Lorem Ipsum, adı
        bilinmeyen bir matbaacının bir hurufat numune
        kitabı oluşturmak üzere bir yazı galerisini
        alarak karıştırdığı 1500'lerden beri endüstri standardı sahte
        metinler olarak kullanılmıştır. Beşyüz yıl
        pek değişmeden elektronik dizgiye de
      </p>
    </div>




  </div>
</template>

<script>


import Post from '@/components/Post'
export default {
  name: "Home",
  components: { Post}
};
</script>

<style scoped>
.home{
  max-width: 605px;
  margin-left: auto;
  margin-right: auto;
  @media (--t) {
    max-width: none;
    display: grid;
    grid-template-columns: 1fr 295px;
    grid-gap: 30px;
  }
}

.sidebar{
  display: none;
  @media (--t) {
    display: block;
    
  }
}
</style>
