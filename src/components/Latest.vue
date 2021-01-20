<template>
    <section class="latest">
        <h3>Latest Posts</h3>
        <div class="posts">

        </div>
    </section>
</template>

<script>
export default {
    name: "latest"
}
</script>

<style lang="scss" scoped>
.latest {
    display: block;
    width: 100%;
    max-width: 1280px;
    margin: 0 auto;

    .posts {
        display: grid;
        // grid-template-columns: 15px  100px  100px  15px;
        grid-template-columns: repeat(4, 1fr);
        grid-template-rows: repeat(3, 195px);
        grid-gap: 25px;

        margin: 15px;

        .post {
            
        }


    }
}
</style>