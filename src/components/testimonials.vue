<template>
    <section class="text-black py-1" id="testimonials">
    <div class="container">
      <h2 class="section-title mx-auto ms-5 ps-5 mx-5 text-center">
        <h1>Testimonial</h1>
      </h2>
      <br />
      <section id="testimonials" class="vh-80">
        <div class="container text-center
        ">
          <div
            id="carouselExampleIndicators"
            class="carousel slide"
            data-bs-ride="carousel"
          >
            <div class="carousel-indicators">
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="0"
                class="active circle"
                aria-current="true"
                aria-label="Slide 1"
              ></button>
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="1"
                aria-label="Slide 2"
                class="circle"
              ></button>
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="2"
                aria-label="Slide 3"
                class="circle"
              ></button>
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="3"
                aria-label="Slide 4"
                class="circle"
              ></button>
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="4"
                aria-label="Slide 5"
                class="circle"
              ></button>
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="5"
                aria-label="Slide 6"
                class="circle"
              ></button>
            </div>
            <div class="card mx-auto pt-4">
            <div class="carousel-inner">
              
                <div class="carousel-item" v-bind:class="{ active: index === 0 }" v-for="(people,index) in people" :key="index" >
                    <img
                  :src="people.image"
                  class="rounded-circle pt-2 pb-2"
                  alt=""
                />
                <h2 class="name">{{ people.name }}</h2>
                <p class="description mx-auto">{{ people.description }}</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>
  </section>
</template>
<script>

export default{
    computed:{
        people(){
          return this.$store.state.people;
        }
    }
}
</script>
<style>
:root {
    --color-primary: #ef1e48;
    --color-white: #aba8a482;
    --color-black: #030910;
    --color-dark: #642330;
    --color-gray: #9d8790;


    --font-Poppins: 'Poppins', sans-serif;
    --font-Raleway: 'Raleway', sans-serif;
    --font-OpenSans: 'Open Sans', sans-serif;

	--font-xlg: 90px;
    --font-lg: 64px;
    --font-md: 26px;
    --font-sm: 15px;
    --font-xs: 9px;

    --size-lg: 1280px;
    --size-md: 976px;
    --size-sm: 768px;
    --size-xs: 500px;
	--size-ms: 200px;
}
#testimonials{
  /* background-color:var(--color-white); */
  background-image: url"https://i.postimg.cc/28JQ19XW/images.jpg";
}
.container{
padding-left:60px;
background-image:url("https://i.postimg.cc/GpndwV4G/1544025-ddd4c.gif");
}
.card{
  height:560px;
  width:400px;
  margin-bottom:50px;
}
h1{
  z-index:-1;
  color:var(--color-dark);
  text-align:center;
  line-height: 90px;
  font-size: var(--font-lg);
  font-weight:var(--size-ms);
  letter-spacing: 0em;
  width: 95%;
  /* margin-bottom: 10px;
  margin-top: 10px; */
}
h2{
  z-index:-1;
  color:var(--color-dark);
  text-align:center;
  font-weight:var(--size-ms);
  font-size: var(--font-lg);

}
.carousel-inner img{
  aspect-ratio: 1;
  object-fit: cover;
  width: 270px;
  height:270px
}
.name{
font-size:23px;
font-weight:400;
}
.carousel-inner{
  height:560px
}
  .circle{
    width: 20px !important;
    height: 20px !important;
    /* aspect-ratio: 1 !important; */
    border-radius: 50% !important;
    /* border-color: var(--color-dark) !important; */
    background-color:var(--color-dark) !important ;
    ;
}

.description{
  width:300px;
}
button .circle{
    height: 10px;
    width:10px;
    margin:0px 0px;
}

</style>