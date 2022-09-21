<template>
    <div>
        <h3>{{msg}}</h3>
        <h3>{{ project.title }}</h3>
        <p>{{ project.description }}</p>
        <a href src={{project.link}}>Link</a>
    </div>
</template>

<script>
export default {
    name: 'ProjectHighlight',
    msg: String,
    description: String,
    projectName: String,
    projectLink: String
}
</script>

<style>

</style>