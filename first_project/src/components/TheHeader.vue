<template>
    <header>
        <div class="container_header">
            <div class="title">Header do Junior</div>
            <div class="icon-1"><img src="https://api.iconify.design/svg-spinners:blocks-scale.svg" alt=""></div>
            <div class="icon-2"><img src="https://api.iconify.design/svg-spinners:blocks-wave.svg" alt=""></div>
        </div>
    </header>
</template>

<script>
export default{

}
</script>

<style>
header{
    /* color: red; */
}
.container_header{
    display: flex;
    flex-direction: column;
    padding: 0%;
    margin: 0%;
    border: 0;
}
.title{
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    color: blue;
    font-size: 120px;
}
.icon-1{
    flex: 1 1 auto;
    flex-direction: row;
    justify-content: center;
    margin: 0% 50%;
    
}

.icon-2{
    flex: 1 1 auto;
    flex-direction: row;
    justify-content: center;
    margin: 0% 50px;
}

img, .icon-1, .icon-2{
    width: 150px;
    right: 150px;
}
</style>
