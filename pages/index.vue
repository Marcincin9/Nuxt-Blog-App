<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest tech news</h1>
    </section>
    <section class="featured-posts">
        <PostPreview 
        id="1"
        thumbnail="https://d26519lbsgqyxd.cloudfront.net/dashboard/wp-content/uploads/2021/02/11155557/lightbulb-illuminating-floor-background.jpg"
        title="Hello there !!"
        previewText="This my first post"/>
        <PostPreview  
        id="2"
        thumbnail="https://d26519lbsgqyxd.cloudfront.net/dashboard/wp-content/uploads/2021/02/11155557/lightbulb-illuminating-floor-background.jpg"
        title="Hello there - secound!!"
        previewText="This my first post"/>
        <PostPreview  
        id="3"
        thumbnail="https://d26519lbsgqyxd.cloudfront.net/dashboard/wp-content/uploads/2021/02/11155557/lightbulb-illuminating-floor-background.jpg"
        title="Hello there - last!!"
        previewText="This my first post"/>
    </section>
  </div>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview.vue'
export default {
 components: {
   PostPreview
 }
 
}
</script>


<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-image: url('~assets/images/bground-pics.jpg');
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}


</style>