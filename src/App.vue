// 置き換わるくさい
<template>
  <div>
    <p>{{ countCharNum }}</p>
    <input v-model="message" />
  </div>
</template>

<script>
// コンポーネントわたすことになってんのか。
export default {
  data: function () {
    return {
      message: "Hello Vue!",
      cnt: "Hello Vue!".length,
    };
  },
  computed: {
    countCharNum: function () {
      return this.message.length;
    },
  },
};
</script>
