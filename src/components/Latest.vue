<template>
    <section class="latest">
        <h3>Latest Posts</h3>
        <div class="posts">
            <div class="post">
                <div class="image" :style="{ backgroundImage: `url(${require('../assets/image1.jpg')})` }"></div>
                <h4>Plan Ahead</h4>
            </div>
            <div class="post col-2 row-2">
                <div class="image" :style="{ backgroundImage: `url(${require('../assets/image2.jpg')})` }"></div>
                <h4>Vue JS fundamentals</h4>
            </div>
            <div class="post row-2">
                <div class="image" :style="{ backgroundImage: `url(${require('../assets/image3.jpg')})` }"></div>
                <h4>Everything wrong with AI </h4>
            </div>
            <div class="post row-2">
                <div class="image" :style="{ backgroundImage: `url(${require('../assets/image4.jpg')})` }"></div>
                <h4>#100daysofcode</h4>
            </div>
            <div class="post">
                <div class="image" :style="{ backgroundImage: `url(${require('../assets/image5.jpg')})` }"></div>
                <h4>NODE package manager</h4>
            </div>
            <div class="post col-2">
                <div class="image" :style="{ backgroundImage: `url(${require('../assets/image6.jpg')})` }"></div>
                <h4>Take a break</h4>
            </div>
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
        grid-template-rows: repeat(3, 196px);
        grid-gap: 30px;

        margin: 15px;

        .image {
            flex: 1;
            background-position: center;
            background-size: cover;
            background-repeat: no-repeat;
        }

        .post {
            display: flex;
            flex-direction: column;

            background-color: #ffffff;
            box-shadow: 3px 3px 8px 0px rgba(0, 0, 0, 0.2); 

            h3{
                box-sizing: border-box;
                padding: 3px 15px 0px 15px;
                height: 50px;
                line-height: 50px;
                margin: 0px;
            }

            &.col-2{
                grid-column: span 2;        
            }            
            &.row-2{
                grid-row: span 2;
            }

        }
    }
}
</style>