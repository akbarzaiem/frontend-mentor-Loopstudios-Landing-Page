<template>
  <div class="cre">
    <!-- font alata -->
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Alata&display=swap"
      rel="stylesheet"
    />
    <!-- font josefin sans -->
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Josefin+Sans:wght@300&display=swap"
      rel="stylesheet"
    />
    <div class="middle-top">
      <div class="left">
        <p>OUR CREATION</p>
      </div>
      <div class="right">
        <button>SEE ALL</button>
      </div>
    </div>
    <div class="middle-bottom">
      <div class="row">
        <div class="item">
          <img src="../assets/desktop/image-deep-earth.jpg" alt="" />
          <p class="desc">DEEP EARTH</p>
        </div>
        <div class="item">
          <img src="../assets/desktop/image-night-arcade.jpg" alt="" />
          <p class="desc">NIGHT ARCADE</p>
        </div>
        <div class="item">
          <img src="../assets/desktop/image-soccer-team.jpg" alt="" />
          <p class="desc">SOCCER TEAM VR</p>
        </div>
        <div class="item">
          <img src="../assets/desktop/image-grid.jpg" alt="" />
          <p class="desc">THE GRID</p>
        </div>
      </div>
      <div class="row">
        <div class="item">
          <img src="../assets/desktop/image-from-above.jpg" alt="" />
          <p class="desc">FROM UP ABOVE VR</p>
        </div>
        <div class="item">
          <img src="../assets/desktop/image-pocket-borealis.jpg" alt="" />
          <p class="desc">POCKET BOREALIS</p>
        </div>
        <div class="item">
          <img src="../assets/desktop/image-curiosity.jpg" alt="" />
          <p class="desc">THE CURIOSITY</p>
        </div>
        <div class="item">
          <img src="../assets/desktop/image-fisheye.jpg" alt="" />
          <p class="desc">MAKE IT FISHEYE</p>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "Creation",
};
</script>

<style scoped>
.middle-top {
  display: flex;
  flex-direction: row;
  margin-top: 80px;
  margin-bottom: 60px;
}
.left {
  justify-content: flex-start;
  flex: 90%;
  margin-left: 10%;
  font-family: "Josefin Sans", sans-serif;
  font-size: 45px;
}
.right {
  row-gap: 500px;
  align-self: center;
  flex: 30%;
  margin-left: -6%;
}
.right button {
  box-sizing: border-box;
  height: 50px;
  width: 190px;
  background-color: transparent;
  border-color: hsl(0, 0%, 55%);
  cursor: pointer;
}
.right button:hover {
  background-color: black;
  color: white;
}
.row {
  display: flex;
  gap: 30px;
  margin-left: 10%;
  margin-bottom: 30px;
}
.row .item img {
  position: relative;
  width: 85%;
}
.row .item {
  cursor: pointer;
}
.row .item :hover {
  opacity: 0.5;
  transform: scale(1.07);
  transition: ease-in-out 1s;
}
.row .desc {
  position: absolute;
  color: white;
  margin-top: -8%;
  margin-left: 2%;
  font-size: 28px;
  width: 128px;
  font-family: "Josefin Sans", sans-serif;
}

@media only screen and (min-width: 320px) and (max-width: 480px) {
  .cre {
    margin-top: 100%;
  }
  .middle-top {
    flex-direction: column;
  }
  .middle-top .left {
    margin-left: 0%;
    width: 100%;
    text-align: center;
  }
  .middle-top .right {
    margin-left: 0%;
    width: 100%;
    display: flex;
    justify-content: center;
  }

  /* image item creation */
  .row {
    flex-direction: column;
    margin-left: 5%;
    margin-right: 5%;
  }
  .row .item img {
    width: 100%;
    max-height: 170px;
    object-fit: cover;
  }
  .row .item .desc {
    margin-top: -20%;
    margin-left: 3%;
    font-size: 28px;
    width: 128px;
  }
  .row .item img:hover {
    opacity: 0.5;
    transform: scale(1.07);
    transition: ease-in-out 1s;
    object-fit: cover;
    max-height: 400px;
  }
}

@media only screen and (min-width: 481px) and (max-width: 768px) {
  .cre {
    margin-top: 120%;
  }
  .middle-top .left {
    margin-left: 5%;
    width: 95%;
    text-align: left;
  }
  .middle-top .right {
    margin-right: 5%;
  }
  /* image item creation */
  .row {
    flex-direction: column;
    margin-left: 5%;
    margin-right: 5%;
  }
  .row .item {
    width: 100%;
  }
  .row .item img {
    width: 100%;
    max-height: 170px;
    object-fit: cover;
  }
  .row .item .desc {
    margin-top: -10%;
    margin-left: 5%;
    font-size: 100%;
    width: 60%;
  }

  .row .item :hover {
    opacity: 0.5;
    transform: scale(1.07);
    transition: ease-in-out 1s;
    object-fit: cover;
    max-height: 400px;
  }
}

@media only screen and (min-width: 769px) and (max-width: 1024px) {
  .row .item .desc {
    margin-top: -10%;
    margin-left: 2%;
    font-size: 150%;
    width: 12%;
  }
}
</style>