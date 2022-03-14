<template>
<div>
    <p>{{ mytext }}</p>
</div>
</template>

<script>
export default {
    data () {
        return {
            mytext: "Text from basic component"
        }
    }
}
</script>

<style>
p {
  font-size: 1.8rem;
  color: blue;
}
</style>