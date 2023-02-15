<template>
<div>
    {{ name }} {{ surn }}
    <button @click="$emit('remove', id)">remove</button>
</div>
</template>

<script>
export default {
    name: "User",
    props: {
    id: Number,
    name: String,
    surn: String,
},
    emits: ["remove"],
};
</script>



<style>
    
</style>