<template>
  <div class="">
    <div class="background1_Box flex">
      <img src="/h5/background1.png" class="background1" />
      <div class="background1Top_content_">
        <div class="background1Top_content">
          <div class="flex topSize">
            <img src="/h5/union.png" class="union" />
            <img src="/h5/unipass.png" class="unipass" />
          </div>
          <div class="flex topSize">
            <span class="span">How it works</span>
            <span class="span">Features</span>
            <el-button class="span topBt">View docs</el-button>
          </div>
        </div>

        <div class="background1Center_content">
          <div>
            <div class="background1_left seedless">
              <div>
                <span>A </span>
                <span class="green">Seedless </span>
                <span>and</span>
              </div>
              <div>
                <span class="green">Gasless</span>
                <span>User</span>
              </div>
              <div>
                <span>Experience for Your</span>
              </div>
              <div>
                <span>Web3 Apps</span>
              </div>
            </div>

            <div class="github_">
              <div class="flex margin">
                <img src="/h5/group.png" class="github" />
                <span> Audited by logo</span>
              </div>
              <div class="flex margin">
                <img src="/h5/github.png" class="github" />
                <span>Open Source</span>
              </div>
            </div>
            <div class="background1Box">
              <el-button class="background1_leftBt">Build now</el-button>
              <el-button class="background1_rightBt">Launch wallet</el-button>
            </div>
          </div>

          <div class="background1_right">
            <img src="/h5/phone.png" class="phone" />
            <img src="/h5/phone1.png" class="phone1" />
            <img src="/h5/phone2.png" class="phone2" />
            <img src="/h5/phone3.png" class="phone3" />
            <img src="/h5/phone4.png" class="phone4" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
useHead({ title: computed(() => $t('Notes')) })
</script>
<style lang="scss">
// background1
.background1_Box {
  position: relative;
  > * {
    z-index: 0;
  }
}
.background1 {
}
.background1Top_content {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
}
.background1Center_content {
  padding: 0 20px 0 0;
  margin-top: 200px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
}
.background1Top_content_ {
  width: 100%;
  max-width: 1200px;
  padding: 0 10px;
  top: 40px;
  z-index: 10;
  position: absolute;
}
.union {
  width: 40px;
  height: 40px;
}
.github {
  width: 24px;
  height: 24px;
  margin-right: 10px;
}
.margin {
  margin-right: 20px;
}
.github_ {
  font-family: 'Open Sans';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  margin-top: 50px;
  color: rgba(255, 255, 255, 0.8);
  flex: none;
  order: 1;
  flex-grow: 0;
  display: flex;
  justify-content: left;
  align-items: center;
}
.flex {
  display: flex;
  justify-content: center;
  align-items: center;
}

.unipass {
  width: 115px;
  height: 18px;
  margin-left: 10px;
}
.span {
  margin-left: 30px;
  color: #fff;
}
.topBt {
  border: 0;
  background: linear-gradient(95.14deg, #b18cff 0%, #8864ff 100%);
  border-radius: 8px;
}
.seedless {
  font-family: 'Futura';
  font-style: normal;
  font-weight: 700;
  font-size: 54px;
  line-height: 70px;
  color: #ffffff;
}
.green {
  color: #acf080;
}

.background1Box {
  margin-top: 30px;
  display: flex;
  justify-content: left;
  align-items: center;
}
.background1_leftBt {
  font-family: 'Open Sans';
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  line-height: 28px;
  padding: 16px 33px;
  width: 201px;
  color: #fff !important;
  height: 60px;
  background: linear-gradient(95.14deg, #b18cff 0%, #8864ff 100%);
  border-radius: 12px;
  border: 0;
  flex: none;
  order: 0;
  flex-grow: 0;
}
.background1_rightBt {
  color: #8864ff;
  font-family: 'Open Sans';
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  line-height: 28px;
  padding: 16px 33px;
  width: 201px;
  height: 60px;
  background: #ffffff;
  box-shadow: inset 2px 1px 4px rgba(255, 255, 255, 0.298432);
  border-radius: 12px;
  /* Inside auto layout */
  flex: none;
  order: 1;
  flex-grow: 0;
}
.background1_right {
}
.phone {
  width: 294px;
  height: 654px;
  position: absolute;
  z-index: 100;
  top: 150px;
  right: 0px;
}

.phone1 {
  width: 67px;
  height: 67px;
  position: absolute;
  z-index: 100;
  top: 345px;
  right: -15px;
}
.phone2 {
  width: 70px;
  height: 71px;
  position: absolute;
  z-index: 100;
  top: 430px;
  right: 255px;
}
.phone3 {
  width: 70px;
  height: 71px;
  position: absolute;
  z-index: 100;
  top: 670px;
  right: 7px;
}
.phone4 {
  width: 180.11px;
  height: 206.39px;
  position: absolute;
  z-index: 100;
  top: 545px;
  right: 230px;
}
// background1
</style>
