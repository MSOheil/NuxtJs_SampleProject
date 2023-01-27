<template>
    <h1>
        joke is :{{ joke }},
        id is :{{ id }}
    </h1>
</template>

<script>
export default {
    name: 'Joke',
    props: ['joke', 'id']
}
</script>

<style>

</style>