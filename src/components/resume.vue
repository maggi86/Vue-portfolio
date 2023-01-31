<template>
<body>
  <section id="resume">
      <div class="timeline">
        <div class="mmm">
        <h1 class="lead text-center">RESUME</h1>
      </div>
        <div class="box left">
          <div class="content">
            <h3>{{resume1[0].date}}</h3>
            <small>
              {{resume1[0].title}}
            </small>
            <p>{{resume1[0].description}}</p>
          </div>
        </div>
        <div class="box right">
          <div class="content">
            <h3>{{resume2[0].date}}</h3>
            <small>
              {{resume2[0].title}}
            </small>
            <p>{{resume2[0].description}}</p>
          </div>
        </div>
        <div class="box left">
          <div class="content">
            <h3>{{resume1[1].date}}</h3>
            <small>
              {{resume1[1].title}}
            </small>
            <p>{{resume1[1].description}}</p>
          </div>
        </div>
        <div class="box right">
          <div class="content">
            <h3>{{resume2[1].date}}</h3>
            <small>
              {{resume2[1].title}}
            </small>
            <p>{{resume2[1].description}}</p>
          </div>
        </div>
        <div class="box left">
          <div class="content">
            <h3>{{resume1[2].date}}</h3>
            <small>
              {{resume1[2].title}}
            </small>
            <p>{{resume1[2].description}}</p>
          </div>
        </div>
        <div class="box right">
          <div class="content">
            <h3>{{resume2[2].date}}</h3>
            <small>
              {{resume2[2].title}}
            </small>
            <p>{{resume2[2].description}}</p>
          </div>
        </div>
        <div class="box left">
          <div class="content">
            <h3>{{resume1[3].date}}</h3>
            <small>
              {{resume1[3].title}}
            </small>
            <p>{{resume1[3].description}}</p>
          </div>
        </div>
        <div class="box right">
          <div class="content">
            <h3>{{resume2[3].date}}</h3>
            <small>
              {{resume2[3].title}}
            </small>
            <p>{{resume2[3].description}}</p>
          </div>
        </div>
      </div>
      <div class="box left">
          <div class="content">
            <h3>{{resume1[4].date}}</h3>
            <small>
              {{resume1[4].title}}
            </small>
            <p>{{resume1[4].description}}</p>
          </div>
        </div>
        <div class="box right">
          <div class="content">
            <h3>{{resume2[4].date}}</h3>
            <small>
              {{resume2[4].title}}
            </small>
            <p>{{resume2[4].description}}</p>
          </div>
        </div>
    </section>
</body>
</template>

<script>
export default{
    computed:{
        resume1(){
          return this.$store.state.resume.resume1;
        },
        resume2(){
          return this.$store.state.resume.resume2;
        }
    }
}

</script>

<style scoped>

:root {
    --color-primary: #ef1e48;
    --color-white: #aba8a482;
    --color-black: #000000;
    --color-dark: #642330;
    --color-gray: #c3c0c1;

    --font-lg: 64px;
    --font-xm: 45px;
    --font-md: 26px;
    --font-sm: 15px;
    --font-xs: 9px;

    --size-lg: 1280px;
    --size-md: 976px;
    --size-sm: 768px;
    --size-xs: 500px;
}


#resume {
  scroll-margin: 100px;
  background-color: var(--color-white);
  padding:20px;
  display:flex;
  justify-content: right;
  margin-left:14%;
  background-image: url("https://i.postimg.cc/GpndwV4G/1544025-ddd4c.gif");
}
* {
  box-sizing: border-box;
  
}
h1{
  z-index:-1;
  color:var(--color-dark);
  text-align:center;
  line-height: 90px;
  font-size: var(--font-lg);
  font-weight:var(--size-ms);
  letter-spacing: 0em;
  width: 95%;}
.mmm p{
  font-size: var(--font-md);
}
.mmm span{
  color: var(--color-primary);
  font-size: var(--font-lg);
}

div .timeline{
  width: 900px;
}


.timeline {
  position: relative;
  max-width: 1000px;
  margin: 0 auto;
}
/* The actual timeline (the vertical ruler) */
.timeline::after {
  content: '';
  position: absolute;
  width: 2px;
  background-color: var(--color-black);
  top: 0;
  bottom: 30px;
  left: 50%;
  margin-left: 0px;
  margin-top: 100px
}
/* Container around content */
.box {
  padding: 10px 40px;
  position: relative;
  width: 50%;
  margin-bottom:40px
}
/* The circles on the timeline */
.box::after {
  content: '';
   position: absolute; 
  width: 15px;
  height: 15px;
  right: -17px;
  background-color: var(--color-primary);
  border: 2px solid var(--color-dark);
  top: 15px;
  border-radius: 50%;
  z-index: 1;
}

p, small{
    color:var(--color-dark);
}

h3{
    color: var(--color-dark);
    font-size:var(--font-md);
}

/* h4{
    color:var(--color-primary);
    font-size: var(--font-lg);
} */

/* Place the container to the left */
.left {
  left: 0;
}
/* Place the container to the right */
.right {
  left: 50%;
}
/* Add arrows to the left container (pointing right) */
.left::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  right: 30px;
  border: medium solid var(--color-gray);
  border-width: 10px 0 10px 10px;
  border-color: transparent transparent transparent var(--color-gray);
}
/* Add arrows to the right container (pointing left) */
.right::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  left: 30px;
  border: medium solid var(--color-gray);
  border-width: 10px 10px 10px 0;
  border-color: transparent var(--color-gray) transparent transparent;
}
/* Fix the circle for containers on the right side */
.right::after {
  left: -16px;
}
/* The actual content */
.content {
  padding: 20px 30px;
  background-color: var(--color-gray);
  position: relative;
}
.content > h3 {
  color:var(--color-primary);
}
@media screen and (max-width:1400px){
  #resume{
    margin-left:0px;
  }
}
@media screen and (max-width: 735px) {
  /* Place the timelime to the left */
  .timeline::after {
  left: 31px;
  }
  /* Full-width containers */
  .box {
  width: 100%;
  padding-left: 70px;
  padding-right: 25px;
  }
  /* Make sure that all arrows are pointing leftwards */
  .box::before {
  left: 60px;
  border: medium solid var(--color-dark);
  border-width: 10px 10px 10px 0;
  border-radius: 1px;
  border-color: transparent var(--color-gray) transparent transparent;
  }
  /* Make sure all circles are at the same spot */
  .left::after, .right::after {
  left: 15px;
  }
  /* Make all right containers behave like the left ones */
  .right {
  left: 0%;
  }
}
</style>