<template>
    <section class="hero">
        <img src="https://picsum.photos/id/180/2400/1600" alt="image">
        <div class="hero-text">
            <h1 class="hero-title">Right now. Write here.
            </h1>
            <p class="hero-subtitle">Place your thoughts on the shelves, remember the important things, be punctual with "Notes"</p>
        </div>
        <div class="hero-overlay"></div>
    </section>
</template>
<script>

export default {
  name:"Hero",
  }

</script>

<style scoped>
.hero {
    position: relative;
    overflow: hidden;
    width: 100%;
    text-align: center;
    display: flex;
    padding: 190px 30px;
    box-sizing: border-box;
}

.hero img {
    position: absolute;
    height: 100%;
    width: 100%;
    object-fit: cover;
    object-position: center;
    top: 0;
    left: 0;
}

.hero-overlay {
    height: 100%;
    width: 100%;
    opacity: 0.6;
    z-index: 2;
    background-color: rgb(12, 12, 12);
    position: absolute;
    top: 0;
    left: 0;
}

.hero-text {
    font-family: Roboto;
    font-weight: 300;
    font-size: 24px;
    line-height: 50px;
    text-align: center;
    z-index: 3;
    color: #FFFFFF;
    display: block;
    position: relative;
    max-width: 780px;
    margin: 0 auto;
}

.hero-title {
    margin: 0;
    margin-bottom: 45px;
}

.hero-subtitle {
    line-height: 1.5;
    font-size: 24px;
    max-width: 580px;
    margin: 0 auto;
}

@media screen and (max-width: 1000px) {
    .hero-subtitle {
        font-size: 20px;
    }
    .hero-title {
        margin-top: 20px;
        font-size: 35px;
    }
    .hero {
        padding: 150px 30px;
    }
}

@media screen and (max-width: 600px) {
    .hero-subtitle {
        font-size: 20px;
    }
    .hero-title {
        margin: 20px 0;
    }
    .hero {
        padding: 100px 30px;
    }
}
    </style>
