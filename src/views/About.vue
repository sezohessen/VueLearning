<template>
    <div class="about">
        <h1>{{ pageName }}</h1>
        <p>{{ pageDesc }}</p>
    </div>
</template>
<script>
// @ is an alias to /src

export default {
    data: function() {
        return {
            pageName: "About Us",
            pageDesc: "This is about us page"
        };
    },
    name: "about",
   /*  directives: {
        bold: {
            bind: el => {
                el.style.fontWeight = "bold";
            }
        }
    } */
};
</script>
