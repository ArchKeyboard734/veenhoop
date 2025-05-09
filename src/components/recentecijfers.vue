<template>
    <!-- waar alle containers in gaat -->
    <div class="maincontainer">
        <!-- linker widget -->
        <div class="container1">
            <!-- binnenin de widget. hier komen later de meest recente cijfers -->
            <div class="cijfers1">

                <label for="vakken">Kies een cijfer:</label>
                <p>input</p>
            </div>

            <div class="button">
                <!-- het stukje  @click="$router.push('naam') is verantwoordelijk voor het doorsturen naar de andere pagina's. in dit geval de cijferlijst pagina -->
                <button @click="$router.push('cijferlijst')">naar cijferlijst</button>
            </div>
        </div>
<!-- rechter widget -->
        <div class="container2">
            <p>input</p>
        </div>
    </div>

</template>
<style scoped>
.container1 {
    display: flex;
    width: 300px;
    height: 300px;
    background-color: darkgray;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    border-radius: 6%;
}

.container2 {
    display: flex;
    width: 300px;
    height: 300px;
    background-color: darkgrey;
    flex-direction: column;
    border-radius: 6%;
}

.cijfers1 {
    display: flex;
    width: 260px;
    height: 260px;
    background-color: lightgray;
    flex-direction: column;
    border-radius: 6%;

}

.maincontainer {
    display: flex;
    width: auto;
    height: auto;
    border-style: dashed;
    border-color: rgb(225, 0, 255);
    justify-content: space-evenly;
    flex-direction: row;
}
</style>