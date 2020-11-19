<template>
    <a-card hoverable style="width: 280px">
        <img 
      slot="cover"
      alt="example"
      :src="src"
    />
    <a-card-meta title="Europe Street beat">
      <template slot="description">
        <p>{{ subMessage }}</p>
          <p class="price">
            {{ price }}
            </p>
      </template>
    </a-card-meta>
          </a-card>
</template>
<style lang="scss" >
.ant-card {
  border-radius: 15px;
}
.ant-card-cover img{
  border-radius: 15px 15px 0 0 ;
}
.ant-card-meta-description
 .price{
   color: #0AC775;
}
</style>
<script>
export default {
  props: {
    mainMessage: {
      type: String,
      default: ''
    },
    subMessage: {
      type: String,
      default: ''
    },
    price: {
      type: String,
      default: ''
    },
    src: {
      type: String,
      default: ''
    }
  }
}
</script>
