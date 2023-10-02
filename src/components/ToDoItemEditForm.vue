<template>
  <form class="stack-small" @submit.prevent="onSubmit">
    <div>
      <label class="edit-label">&quot;{{ "label" }}&quot;の名前を編集</label>
      <input :id="id" ref="labelInput" type="text" autocomplete="off" />
    </div>
    <div class="btn-group">
      <button type="button" class="btn">キャンセル</button>
      <button type="submit" class="btn btn__primary">保存</button>
    </div>
  </form>
</template>
<script>
export default {
  props: {
    id: {
      type: String,
      required: true,
    },
  },
};
</script>
<style scoped>
.edit-label {
  font-family: Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #0b0c0c;
  display: block;
  margin-bottom: 5px;
}
input {
  display: inline-block;
  margin-top: 0.4rem;
  width: 100%;
  min-height: 4.4rem;
  padding: 0.4rem 0.8rem;
  border: 2px solid #565656;
}
form {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}
form > * {
  flex: 0 0 100%;
}
</style>
