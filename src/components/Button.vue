<template>
  <div class="page">
    <button
      class="page__button"
      @click="showPopUpInfo"
    >
      Create new boot
    </button>

  </div>
</template>

<script>

export default {
  name: 'Button',
  components: {

  },
  methods: {
    showPopUpInfo() {
      this.$emit('showPopUp');
    },
  },
};
</script>

<style lang="scss">
.page {

  margin-bottom: 40px;

  line-height: 100px;
  font-family: "Montserrat", sans-serif;
  font-size: 32px;
  font-weight: semibold;

  &__button {
  position: relative;
  width: 400px;
  height: 100px;
  margin-bottom: 25px;
  border-radius: 32px;

  background-color: #f3f0f1;
  border: none;
  color: #6f6cde;
  box-shadow: -6px -6px 10px rgba(255, 255, 255, 0.8),
  6px 6px 10px rgba(0, 0, 0, 0.2);
  text-align: center;
  cursor: pointer;
  transition: all 0.1s ease-in-out;
  }

  &__button:hover {
    opacity: 0.3;
    box-shadow: -6px -6px 10px rgba(255, 255, 255, 0.8),
      6px 6px 10px rgba(0, 0, 0, 0.2);
  }

  &__button:active {
    opacity: 1;
    box-shadow: inset -4px -4px 8px rgba(255, 255, 255, 0.5),
      inset 8px 8px 16px rgba(0, 0, 0, 0.1);
    color: #79e3b6;
  }
}
</style>
