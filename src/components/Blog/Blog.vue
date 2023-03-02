/<template>
  <div class="blogContainer">
    <div class="blogTop">
        <div class="blogHeader">
            <div class="blogHeaderSecondary">
                <div class="blogHeaderLeft">
                    <p>BLOG</p>
                </div>
                <div class="blogArrow">
                    <i class="gg-arrow-left"></i>
                    <i class="gg-arrow-right"></i>
                </div>
            </div>
            <p class="blogHeaderMain">Explore <span class="backgroundText">Marketing</span> Tips</p>
        </div>
    </div>
    <div class="trainingTipsContainer">
        <div v-for="item in marketingTipsOptions"
        :key="item.ID">
            <TipsOptions class="trainingTipsOptions" :tips="item"></TipsOptions>
        </div>
    </div>
  </div>
</template>

<script>
import { isProxy, reactive, toRaw } from 'vue';
import marketingTips from "./../../constants/blogResource"
import TipsOptions from "./TipsOptions/TipsOptions.vue"
export default { 
    components:{
        TipsOptions
    }, 
    data(){
        return{
            marketingTipsOptions: [],
            test:{
                name:"jaj"
            }
        }
    },
    created(){
        this.marketingTipsOptions = [...marketingTips]
    }
}
</script>

<style>
.blogContainer{
    height: 731px;
    background: #FFFFFF;
}
.trainingTipsContainer{
    padding:42px 191px 64px 191px;
    display: flex;
    gap:24px;
}
.trainingTipsOptions{
    
    width: 312px;
    height: 487px;
    background: #FFFFFF;
}
.blogHeaderMain{
    width: 400px;
    height: 40px;
    /* UI Properties */
    text-align: left;
    font: normal normal bold 32px/42px Merriweather;
    letter-spacing: 0.5px;
    color: #1E202F;
    opacity: 1;
}
.blogTop{
    padding:98px 193px 0px 191px;
}
.blogHeaderSecondary{
    display: flex;
    justify-content: space-between;
}
.blogHeaderSecondary p{
    text-align: left;
    font: normal normal bold 14px/26px Muli;
    letter-spacing: 1px;
    color: #4099F1;
    opacity: 1;
}
.blogArrow{
    display: flex;
    gap: 24px;
}
.gg-arrow-left {
    box-sizing: border-box;
    position: relative;
    display: block;
    transform: scale(var(--ggs,1));
    width: 22px;
    height: 22px
}
.gg-arrow-left::after,
.gg-arrow-left::before {
    content: "";
    display: block;
    box-sizing: border-box;
    position: absolute;
    left: 3px
}
.gg-arrow-left::after {
    width: 8px;
    height: 8px;
    border-bottom: 2px solid;
    border-left: 2px solid;
    transform: rotate(45deg);
    bottom: 7px;
    opacity: 0.2;
}
.gg-arrow-left::before {
    width: 24px;
    height: 2px;
    bottom: 10px;
    background: currentColor;
    opacity: 0.2;
}
.gg-arrow-right {
    box-sizing: border-box;
    position: relative;
    display: block;
    transform: scale(var(--ggs,1));
    width: 22px;
    height: 22px;
    color:#4099F1;
}
.gg-arrow-right::after,
.gg-arrow-right::before {
    content: "";
    display: block;
    box-sizing: border-box;
    position: absolute;
    right: 3px
}
.gg-arrow-right::after {
    width: 8px;
    height: 8px;
    border-top: 2px solid;
    border-right: 2px solid;
    transform: rotate(45deg);
    bottom: 7px
}
.gg-arrow-right::before {
    width: 24px;
    height: 2px;
    bottom: 10px;
    background: currentColor
}
</style>