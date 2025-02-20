<template>
    <footer class="footer">
        <div class="footer-content">
            <div class="flag1">Flag 1</div>
            <div class="flag2">Flag 2</div>
            <div class="flag3">Flag 3</div>
        </div>
    </footer>
</template>

<script>
    export default{

    }
</script>

<style>
.footer{
    border: 0px;
    padding: 0px;
    margin: 0px;
}
.footer-content{
    width: 100%;
    height:100px;
    display:flex;
    flex-direction: column;
    background-color: blanchedalmond;
}
.flag1{
    color: chocolate;
    font-family: Georgia, 'Times New Roman', Times, serif;
}
.flag2{
    color: aquamarine;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}
.flag3{
    color: coral;
    font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
}

</style>