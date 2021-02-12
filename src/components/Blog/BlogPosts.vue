<template>
    <div class="post-box">
        <span class="post-views">120</span>
        <h3 class="post-title">Blog post title</h3>
        <span class="post-date">1-1-2021</span>
        <p class="post-constant">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quasi
            quae, deserunt illum tempora adipisci ex quas vitae blanditiis,
            quaerat consectetur placeat facilis? Doloremque velit quibusdam
            cupiditate similique magni id aliquid.
        </p>
        <div class="row">
            <div class="col-md-6">
                <span class="post-author">Post author</span>
            </div>
            <div class="col-md-6 text-right">
                <span class="post-category">Category Name</span>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: "post"
};
</script>
<style lang="scss" scoped>
.post-box {
    padding: 15px;
    background-color: #fff;
    box-shadow: 0 0 10px #ddd;
    position: relative;
    text-align: left;
    .post-views {
        position: absolute;
        top: 5px;
        right: 5px;
        background-color: #4fa523;
        border-radius: 4px;
        padding: 3px;
        color: #fff;
        text-align: center;
        font-weight: bold;
    }
    .post-title {
        font-weight: bold;
        padding: 15px;
    }
    .post-date {
        padding: 0 0 5px;
        display: block;
        color: #888;
        font-size: 14px;
    }
    .post-constant {
        line-height: 1.8;
        color: #666;
    }
    .post-author {
        background-color: #291919;
        padding: 6px 10px;
        border-radius: 4px;
        color: #fff;
    }
    .post-category {
        background-color: #c52828;
        padding: 6px 10px;
        border-radius: 4px;
        color: #fff;
    }
}
</style>
