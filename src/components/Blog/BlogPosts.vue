<template>
    <div class="post-box" id="post">
        <span class="post-views">{{ views }}</span>
        <h3 class="post-title">{{ title }}</h3>
        <span class="post-date">{{ date }}</span>
        <p class="post-constant">
            {{ content }}
        </p>
        <div class="row">
            <div class="col-md-6">
                <span class="post-author">{{ author }}</span>
            </div>
            <div class="col-md-6 text-right">
                <span class="post-category">{{ uppercase(category) }}</span>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data: function() {
        return {
            uppercase: v => {
                return v.toUpperCase();
            }
        };
    },
    props: ["views", "title", "date", "content", "author", "category"],
    name: "post"
};
</script>
<style lang="scss" scoped>
.post-box {
    margin-bottom: 20px;
    padding: 20px;
    background-color: #fff;
    box-shadow: 0 0 10px #ddd;
    position: relative;
    border-radius: 2px;
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
