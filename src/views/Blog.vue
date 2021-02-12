<template>
    <div class="our-blog">
        <h1>{{ pageName }}</h1>
        <p>{{ pageDesc }}</p>
        <div class="container">
            <div class="row">
                <div class="col-md-8">
                    <div class="posts-area">
                        <blog-posts />
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="side-bar">
                        <blog-side-bar/>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import BlogPosts from '../components/Blog/BlogPosts.vue';
import BlogSideBar from '../components/Blog/BlogSideBar.vue';

export default {
  components: { BlogPosts, BlogSideBar },
    data: function() {
        return {
            pageName: "Blog",
            pageDesc: "This is blog page"
        };
    },
    name: "blog",
    
};
</script>
