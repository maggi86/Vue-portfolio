<template>
    <section class=" text-black py-5" id="testimonials">
    <div class="container">
      <h2 class="section-title">
        <center>Testimonial</center>
      </h2>
      <br />
      <section id="testimonials" class="vh-80">
        <div class="container text-center p-5">
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
            <div class="carousel-inner pb-5">
                <div class="carousel-item" v-bind:class="{ active: index === 0 }" v-for="(people,index) in people" :key="index" >
                    <img
                  :src="people.image"
                  class="rounded-circle"
                  alt=""
                />
                <p>{{ people.name }}</p>
                <p>{{ people.description }}</p>
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
    --color-white: #e8e6e3;
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
  background-color:var(--background-color)
}
.carousel-inner img{
  aspect-ratio: 1;
  object-fit: cover;
  width: 300px;
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


button .circle{
    height: 10px;
    width:10px;
    margin:0px 0px;
}

</style>