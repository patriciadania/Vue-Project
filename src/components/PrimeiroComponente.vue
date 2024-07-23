<template>
    <div>
    <h1> OLA VUE</h1>
    <p> Meu nome é {{ nome }} </p>
    </div>
</template>

<script>
export default{
    name: "PrimeiroComponente",
    data() {
        return {
            nome: "Patricia",
        }
    }
}

</script>