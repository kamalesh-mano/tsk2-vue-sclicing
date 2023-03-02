<template>
  <div class="footerContainer">
    <div class="leftFooter">
        <img class="footerLogo" src="../../assets/Logo.svg" alt="LOgo">
        <a href="/" class="footerTerms">Terms & Condition</a>
        <a href="/">Privacy Policy</a>
    </div>
    <div class="rightFooter">
        <p>® 2019 Company name. All rights reserved.</p>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.footerTerms{
    padding-right:33px;
}

.footerLogo{
    width: 148px;
    height: 58px;
    padding-right: 13px;
}
.footerContainer{
    display: flex;
    justify-content: space-between;
    height: 142px;
    background: #FFFFFF;
    align-items: center;
    padding: 0 192px
}
a{
    text-decoration: none;
}
.rightFooter{
    width:342px;
    text-align: right;
    font: normal normal normal 16px/26px Muli;
    letter-spacing: 0.5px;
    color: #82868A;
    opacity: 1;
}
.leftFooter{
    display: flex;
    align-items: center;
    gap:33px
}
</style>