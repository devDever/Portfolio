<template>
  <div>
    <div class="container">
      <div class="main_home__wrapper">
        <div class="top_side">
          <div class="main_title">
            <h1>ISA</h1>
          </div>
        </div>
        <div class="bottom_side">
          <img src="@/assets/me.jpg" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {},
};
</script>

<style lang="scss">
.main_home__wrapper {
  padding-top: 30px;
  height: 95vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  .top_side {
    h1 {
      font-size: 70px;
      font-family: "main-font-bold";
      font-weight: bold;
    }
  }
  .bottom_side {
    margin-top: 30px;
    img {
      width: 100%;
    }
  }
}
</style>
