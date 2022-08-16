<!-- @format -->
<script setup lang="ts">
  const onClick = () => {
    console.log("click");
  };
</script>
<template>
  <div class="container">
    <div class="form">
      <div class="from-top">
        <p id="txtTitle"><span id="txtYou">You</span>topia</p>
      </div>
      <div @click="onClick()" class="btnGoogle">
        <img
          class="image"
          src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Google_%22G%22_Logo.svg/768px-Google_%22G%22_Logo.svg.png"
        />
        <span class="txtLoginWithGoogle"> Login with google </span>
      </div>
      <div class="container-line">
        <div class="line"></div>
        <span class="text">OR</span>
        <div class="line"></div>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .container {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
    justify-content: center;
  }
  .form {
    width: 25vw;
    height: 30vw;
    background-color: wheat;
    align-self: center;
    border-radius: 1vw;
    flex-direction: column;
    display: flex;
  }
  #txtYou {
    color: darkcyan;
  }
  #txtTitle {
    font-size: 1.5vw;
    font-weight: bold;
    align-self: center;
    text-align: center;
  }
  .image {
    width: 1.5vw;
    height: 1.5vw;
    margin: 0px 10px;
  }

  .text {
    color: gray;
  }
  .container-line {
    width: auto;
    height: 3vh;
    overflow: hidden;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
  }
  .line {
    height: 1px;
    width: 30%;
    background-color: gray;
    margin: 0px 15px 0px 15px;
  }
  .btnGoogle {
    width: 85%;
    height: 50px;
    border-color: black;
    border-radius: 1rem;
    border-width: 1px;
    border-style: solid;
    align-self: center;
    display: flex;
    justify-content: center;
    align-items: center;
  }
</style>
