<template>
    <main>
        <div class="container-forms">
            <form action="../../register/cadastro.txt" method="get">
                <div class="subtitle-forms"><h3>Forms do Legal!</h3></div>
                <input type="text" value="Seu nome">
                <div div="subtitle-forms"><h3>Você é legal?</h3></div>
                <input type="checkbox" name="sim-legal" id="legal"> Sim
                <input type="checkbox" name="nao-legal" id="não-legal"> Não
                <input type="submit" value="Enviar">
            </form>
        </div>
    </main>
</template>

<script>
export default{

}

</script>

<style>
.container-forms{
    display: flex;
    flex-direction: column 5rem;
    justify-content: center;
    background-color: rgba(0, 0, 0, 0.63);
    right: 500px;
    width: 500px;
    border-radius: 2rem;
    margin: 2px 2px 2px 2px;
    padding: solid;
}
.sutitle-forms{
    flex-direction: column;
    justify-content: center;
}
</style>