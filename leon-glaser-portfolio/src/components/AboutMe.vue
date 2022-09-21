<template>
    <div>
        <h3>{{label}}</h3>
        <p>{{ msg }}</p>
    </div>

</template>

<script>
export default {
    name: 'AboutMe',
    props: {
        label: String,
        msg: String
    }
}
</script>

<style>

</style>