<template>
  <div class="exhibitions-wrap">
        <article class="exhibition-listing odd">
            <a class="wrap" target="_blank" href="https://github.com/cheer4chai/best-chinese-front-end-blogs">
                <div class="text firstText">
                    <h3>优质中文前端博客</h3>
                    <p class="link">Info</p>
                </div>
                <div class="image-wrap">
                    <div class="image-wrap2">
                    <div class="image">
                        <img src="../../assets/blog.png" width="210" height="210" alt="">
                        </div>
                    </div>
                </div>
            </a>
        </article>
        <article class="exhibition-listing even">
            <a class="wrap" target="_blank" href="https://github.com/cheer4chai/Front-end-Interview-questions">
                <div class="text">
                    <h3>前端面试知识点</h3>
                    <p class="link">Info</p>
                </div>
                <div class="image-wrap">
                    <div class="image-wrap2">
                    <div class="image">
                        <img src="../../assets/interview.png" width="210" height="210" alt="">
                        </div>
                    </div>
                </div>
            </a>
        </article>
        <footer id="footer"></footer>
  </div>
  
</template>

<script>
export default {
  name: 'resource'
}
</script>

<style scoped>
body .exhibitions-wrap {
    text-align: center;
}
.exhibition-listing {
    margin: 70px 0 auto;
    position: relative;
}
.exhibition-listing .text:before {
    content: '';
    position: absolute;
    background: #000;
    width: 5px;
    height: 70px;
    left: 50%;
    margin-left: -2px;
    top: -70px;
}
.exhibition-listing .firstText:before {
    content: '';
    position: absolute;
    background: #000;
    width: 5px;
    height: 100px;
    left: 50%;
    margin-left: -2px;
    top: -100px;
}

.exhibition-listing .text {
    border: 5px solid #000;
    padding: 30px;
    width: 370px;
    margin: 0 auto;
    text-align: center;
    font-size: 18px;
}
.exhibition-listing.odd .image-wrap {
    right: 50%;
    margin-right: 300px;
}
.exhibition-listing.even .image-wrap {
    left: 50%;
    margin-left: 300px;
}
.exhibition-listing .image-wrap {
    position: absolute;
    top: -50px;
}
.exhibition-listing.odd .image-wrap:after {
    content: '';
    position: absolute;
    background: #000;
    height: 5px;
    width: 120px;
    bottom: 50%;
    right: -115px;
}
.exhibition-listing.even .image-wrap:after {
    content: '';
    position: absolute;
    background: #000;
    height: 5px;
    width: 120px;
    bottom: 50%;
    left: -115px;
}
.exhibition-listing .image-wrap .image-wrap2 {
    display: table-cell;
    vertical-align: middle;
    height: 240px;
}
.exhibition-listing .image-wrap .image-wrap2 .image {
    margin-bottom: 0;
    background: #fff;
    border: 5px #000 solid;
    padding: 10px;
    margin: 0 0 50px;
    display: inline-block;
}

.exhibition-listing .image-wrap .image-wrap2 .image img{
    width: 180px;
    height: 180px;
}

</style>
