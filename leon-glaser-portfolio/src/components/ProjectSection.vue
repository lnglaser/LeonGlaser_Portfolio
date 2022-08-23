<template>
    <h1>Projects</h1>
    <h2>{{ msg }}</h2>
    <!-- <p>{{ projects }}</p> -->
    <div :key="project.id" v-for="project in projects">
        <h3>{{ project.title }}</h3>
        <p>{{ project.description }}</p>
        <a href={{project.link}}>Link</a>
    </div>
</template>

<script>

export default {
    name: 'ProjectSection',
    props: {
        msg: String,
        projects: Array
    }
}

</script>

<style>
</style>