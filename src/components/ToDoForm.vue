<template>
  <form>
    <h2 class="label-wrapper">
      <label for="new-todo-input" class="label__lg">
        タスクを入力してください
      </label>
    </h2>
    <input
      type="text"
      id="new-todo-input"
      name="new-todo"
      autocomplete="off"
      class="input__lg" />
    <button type="submit" class="btn btn__primary btn__lg">追加する</button>
  </form>
</template>

<script>
export default {
  methods: {
    onSubmit() {}, // タスクの追加
  },
};
</script>
