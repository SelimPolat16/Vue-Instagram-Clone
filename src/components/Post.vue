<template>
  <div class="post">

    <!-- Header -->
    <header class="header section">

      <div class="header-author">
        <Avatar :size="40" />
        <div class="header-author-info">
          <div>
            <CustomText tag="b">selimpolat16</CustomText>
          </div>
          <div>
            <CustomText size="xsmall">Bursa, Yıldırım</CustomText>
          </div>
        </div>
      </div>
      <div class="header-more">
        <button type="button">
            <IconMore />
        </button>
      </div>
    </header>

    <!-- media -->
      <div class="post-media">
          <img src="https://instagram.fyei1-1.fna.fbcdn.net/v/t51.2885-15/sh0.08/e35/p640x640/118873019_318232429624017_7026074334175624797_n.jpg?_nc_ht=instagram.fyei1-1.fna.fbcdn.net&_nc_cat=109&_nc_ohc=dvtszVOSZXMAX-RM2hd&oh=7bb144e22235a18e93b693630a0188d3&oe=5F7F36A0"
          alt="">
      </div>
    <!-- actions  -->
    <div class="actions-buttons section">
      <button type="button">
        <IconLike />
      </button>
      <button type="button">
        <IconComment />
      </button>
      <button  type="button">
        <IconDirect />
      </button>
      <button class="action-save" type="button">
        <IconSave />
      </button>
    </div>
    <!-- wiew count -->
    <div class="wiew count section">
      <custom-text tag="b">1.700 beğenme</custom-text>
    </div>

    <!-- comment list -->

    <!-- datetime -->

    <!-- comment form -->
  </div>
</template>

<script>
import Avatar from '@/components/Avatar'
import CustomText from '@/components/CustomText'
import IconMore from '@/icons/more.svg'
import IconLike from '@/icons/like.svg'
import IconComment from '@/icons/comment.svg'
import IconDirect from '@/icons/direct.svg'
import IconSave from '@/icons/save.svg'
export default {
  name: 'Post',
  components: {
    IconLike,
    IconComment,
    IconDirect,
    IconSave,
    IconMore,
    CustomText,
    Avatar }
}
</script>

<style scoped>
.post{
  border-radius: 3px;
  border: 1px solid rgb(var(--b6a));

}
.section{
  padding-left: 16px;
  padding-right: 16px;
}
.header{
  height: 60px;
  display: flex;
  align-items: center;

  &-author{
    display: flex;
    align-items: center;

    &-info{
      margin-left: 16px;
    }
  }

  &-more{
    margin-left: auto;
  }
}

.actions-buttons{
  height: 45px;
  display: flex;
  align-items: center;

  button{
    margin-right: 16px;
  }

  .action-save{
    margin-left: auto;
    margin-right: 0;
  }
}

</style>