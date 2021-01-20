<template>
    <div class="posts">
        <button class="load">See more</button>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.posts {
    width: 100%;
    max-width: 1280px;
    margin: 50px auto;

    .load {
        display: block;
        width: 100%;
        max-width: 250px;
        height: 50px;

        margin: 0 auto;

        outline: none;
        border: none;
        border-radius: 10px;
        appearance: none;

        background-color: #ffce00;
        box-shadow: 3px 3px 8px 3px rgba(0, 0, 0, 0.2);
        box-sizing: border-box;

        color: #171717;
        font-family: 'Rockwell', serif;
        font-size: 28px;
        font-weight: 700;
    }
}
</style>