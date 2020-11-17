<template>
  <div class="gutter-example">
    <a-row :gutter="16">
      <a-col class="gutter-row" :span="6">
        <div class="gutter-box">
          <a-card hoverable style="width: 240px">
        <img
      slot="cover"
      alt="example"
      :src="src"
    />
    <a-card-meta title="Europe Street beat">
      <template slot="description">
        <p>{{ subMessage }}</p>
          <p class="price"></p>
            {{ price }}
      </template>
    </a-card-meta>
  </a-card>
        </div>
      </a-col>
      <a-col class="gutter-row" :span="6">
        <div class="gutter-box">
          col-6
        </div>
      </a-col>
      <a-col class="gutter-row" :span="6">
        <div class="gutter-box">
          col-6
        </div>
      </a-col>
      <a-col class="gutter-row" :span="6">
        <div class="gutter-box">
          col-6
        </div>
      </a-col>
    </a-row>
  </div>
</template>
<style lang="scss" scoped>
.gutter-example >>> .ant-row > div {
  background: transparent;
  border: 0;
}
.gutter-box {
  padding: 5px 0;
}
</style>
<script>
export default {
  props: {
    mainMessage: {
      type: String,
      default: ' '
    },
    subMessage: {
      type: String,
      default: ' '
    },
    price: {
      type: String,
      default: ''
    },
    src: {
      type: String,
      default: ' '
    }
  }
}
</script>
