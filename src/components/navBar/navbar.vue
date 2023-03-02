<script>
export default{
}
</script>

<template>
    <div class="navContainer">
        <div class="leftNav">
            <img src="../../assets/Logo.svg" alt="LOgo">
        </div>
        <div class="rightNav">
            <div class="menuOptions">
                <a href="/">Why us?</a>
                <a href="/">Marketing Platform</a>
                <a href="/">Pricing</a>
                <button class="signUpButton">Sign Up,its Free</button>
            </div>
        </div>
    </div>
</template>

<style scoped>
.navContainer{
    display: flex;
    justify-content: space-between;
    height: 100px;
    background: #FFFFFF;
    align-items: center;
    padding: 0 192px;
}
.menuOptions{
    display: flex;
    gap: 32px;
    align-items: center;
}
a{
    text-decoration: none;
}
.signUpButton{
    background: #FFFFFF;
    border: 1px solid #4099F1;
    opacity: 1;
    width: 132px;
    height: 42px;
    text-align: center;
    font: normal normal normal 14px/11px Muli;
    letter-spacing: 0px;
    color: #4099F1;
}
</style>
