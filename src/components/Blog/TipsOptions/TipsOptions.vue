<template>
    <div class="optionContainer">
        <div class="optionImage">
            <img :src=tips.Image alt="landing Image">
        </div>
        <div class="optionHeader">{{ tips.Header }}</div>
        <div class="optionInfo">{{ tips.INFO }}</div>
        
    </div>
  
</template>

<script>
import { isProxy, toRaw } from 'vue';
export default {
    props: ["tips"],
    setup(props) {
        console.log(props.tips)
  }
}
</script>

<style>
img{
    width: 312px;
    height: 322px;
}
.optionHeader{
    width: 257px;
    height: 55px;
    text-align: left;
    font: normal normal 900 20px/30px Merriweather;
    letter-spacing: 0.42px;
    color: #1E202F;
    opacity: 1;
    padding: 24px 55px 0px 0px;
}
.optionInfo{
    width: 312px;
    height: 70px;
    text-align: left;
    font: normal normal normal 12px/23px Muli;
    letter-spacing: 0.24px;
    color: #888990;
    opacity: 1;
    padding: 16px 55px 0px 0px;
}
</style>