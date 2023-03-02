<template>
  <div class="landingPageContainer">
    <div class="landingPageInfo">
        <div class="infoText">
            <p>We take care Marketing things</p>
        </div>
        <div class="infoButton">
            <button>Pick a Plan</button>
        </div>
    </div>
    <div class="landingPageImage">
        <img src="../../assets/Illustration@2x.png" alt="landing Image">
    </div>
  </div>
</template>

<script>

export default {
    
}
</script>

<style scoped>
.landingPageContainer{
    height:668px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding: 63px 47px 63px 191px;
}
img{
    width: 636px;
    height: 542px;
    padding:63px 0px 63px 0px;
}
.landingPageInfo{
    padding: 156px 0px 156px 0px;
    width: 480px;
    height: 356px;
}
.infoText{
    height: 272px;
    text-align: left;
    font: normal normal bold 64px/90px Merriweather;
    letter-spacing: 0.45px;
    color: #1E202F;
    opacity: 1;
    padding-bottom: 32px;
}
.infoButton button{
    height: 52px;
    width: 144px;
    background: #4099F1 0% 0% no-repeat padding-box;
    opacity: 1;
    color: #FFFFFF;
    border: none;
}
</style>