<template>
  <div class="card__wrapper">
    <div class="card__text">
      <p>Merry</p>
      <p>Christmas!</p>
    </div>
    <div class="card">
      <div class="snow"></div>
      <div class="snow"></div>

      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
      <div class="snow"></div>
    </div>
  </div>
</template>
<script setup lang="ts">

</script>
<style lang="scss" scoped>
.card__wrapper {
  position: absolute;
  bottom: 0;
  left: 50%;
  .card {
    $snow-size: 2em;
    width: $snow-size * 10;
    height: $snow-size * 10;
    padding: 2em;
    display: flex;
    flex-wrap: wrap;
    filter: blur(15px);

    .snow {
      position: relative;
      width: $snow-size;
      height: $snow-size;
      border-radius: 100%;
      filter: contrast(30);

      &::after {
        position: absolute;
        content: "";
        left: 0;
        width: inherit;
        height: inherit;
        background: white;
        transition: 30s cubic-bezier(0.19, 1, 0.22, 1);
      }

      &:hover::after {
        transform: scale(0);
        transition-duration: 0.1s;
      }
    }
  }

  .card__text {
    position: absolute;
    top: 25%;
    left: 50%;
    z-index: 9999;
    color: white;
    font-weight: 600;
    font-size: 24px;
    line-height: 1em;
    letter-spacing: 0.1em;
    transform: translate(-50%, -30%);
    pointer-events: none;
    filter: blur(1px) contrast(20);
    text-align: center;
    p {
      margin-bottom: 12px;
    }
  }
}
</style>