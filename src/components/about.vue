<template>
<body>
  <div class="container">
    <div class="row">
      <div class="col-md-12 about-panel-wrapper">
      	<div class=" about-panel animated fadeIn">
  	      <div class="perspective-container">
  		      <div class="zero photo-about animated fadeIn"> 
  		        <div class="hide-photo-filter animated fadeIn"></div>
  		        <div class="about-info">
  		        	<h3 class="about-info-name animated fadeInUp up-one">Meagan Williams</h3>
  		        	<div class="about-info-contact">
  		        		<h4 class="animated fadeInUp up-two"> An Aspiring Web developer</h4>
  		        		<a>meaganwilliams407@gmail.com</a>
  		        	</div>
  		        </div>
  		      </div>
  	      </div>
      	</div>
      </div>
    	<div class="col about-content " >
    	  <div class="about-me mx-auto text-center" >
    	  <h1 class="animate fadeIn one mx-2">ABOUT</h1>
    	    <div class="animated fadeIn two">
    	      <p class="lead text-center fw-bold m-3">Hungry, resilient, driven and tenacious. That's how I'd describe myself. When I'm not busy coding and compiling, I'm spending time reading, watching a lot of tv or learning more about things I dont know. Below you'll find my key performance areas as well as my current skill stack, with <span>HTML</span>, <span>CSS</span>, <span>Mysql</span>, <span>JavaScript</span>, <span>Vue.js</span> and <span>Bootstrap</span> as my core skills.</p>
        		<p class="lead text-center fw-bold m-3">
          	My hobbies include baking and cooking. I like reading books on my phone or online. I like trying new things such as food and activities. I enjoy music, not in the sense where I can make it but I love listening to music when doing things.
					  </p>
    	    </div>
					<div class="container text-center ms-4">
        		<h3>SKILL STACK</h3>
        		<!-- <br> -->
        		<div class="row d-flex justify-content-center align-items-center flex-row">
          		<div class="col rounded border border-1 p-3 me-5 mx-lg-5 my-3">
            		<img src="https://i.postimg.cc/gjnyV8Hb/7422531-css3-css-file-development-icon.png">
            		<p>CSS3</p>
          	  </div>
          		<div class="col rounded border border-1 p-3 me-5 mx-lg-5 my-3">
            		<img src="https://i.postimg.cc/c4Ckh8LH/367627-html-html5-icon.png">
            		<p>HTML5</p>
          		</div>
          		<div class="col rounded border border-1 p-3 me-5 mx-lg-5 my-3">
            		<img src="https://i.postimg.cc/Kj230WLb/8666135-bootstrap-icon.png">
            		<p>BOOTSTRAP</p>
          		</div>
              <div class="col rounded border border-1 p-3 me-5 mx-lg-5 my-3">
            		<img src="https://i.postimg.cc/wvnYz4Kr/4691303-mysql-icon.png">
            		<p>MYSQL</p>
          	  </div>
          		<div class="col rounded border border-1 p-3 me-5 mx-lg-5 my-3">
            		<img src="https://i.postimg.cc/qvwCBSJg/8666390-js-square-icon.png">
            		<p>JAVASCRIPT</p>
          		</div>
          		<div class="col rounded border border-1 p-3 me-5 mx-lg-5 my-3">
            		<img src="https://i.postimg.cc/kgJBHsQC/9055767-bxl-vuejs-icon.png">
            		<p>VUE.JS</p>
          		</div>
              <div class="col rounded border border-1 p-3 me-5 mx-lg-5 my-3">
            		<img src="https://i.postimg.cc/pTnFmT9b/icons8-wordpress-24.png">
            		<p>WORDPRESS</p>
          		</div>
              <div class="col rounded border border-1 p-3 me-5 mx-lg-5 my-3">
            		<img src="https://i.postimg.cc/3rcqMbhk/icons8-php-logo-100.png">
            		<p>PHP</p>
          		</div>
              
        		</div>
      		</div>
    	  </div>
    	</div>
      
    </div>
  </div>
</body>
</template>

<style scoped>

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
 

body {
  /* font-family: "Helvetica Neue", Helvetica, Arial, sans-serif; */
  
  /* line-height: 1.19; */
  color: var(--color-gray);
  background-color: var(--color-white);
    width: 100%;
	max-width: 100%;
  background-image: url("https://i.postimg.cc/GpndwV4G/1544025-ddd4c.gif");
}

span{
  color: var(--color-primary);
}

.about-content, .about-panel {
  max-width: 50%;
	width: 50%;
  margin-left:175px
}

.container {
  margin: 0;
  padding: 0;
  font-size: 25px;
  font-weight:bold;
  letter-spacing: 0.3px;
	/* background-image: url("https://i.postimg.cc/sDjnJCtj/Meagan-2.jpg") no-repeat; */
  overflow-y: auto;
overflow-x:hidden ;
  height: 100%;
	max-width: 100%;
}


.about-panel {
  padding: 0;
  position: absolute;
	top:0;
	right:0;
  -webkit-animation: example 1.2s both ease-in;
  -moz-animation: example 1.2s both ease-in;
  animation: example 1.2s both ease-in;
	height: 100vh;
  width:43%;
}
p {
  font-size:20px;
  /* font-weight: bold; */
}
h3{
  font-size:30px;
  font-weight:bold;
  margin-top:20px;
}

.about-panel .photo-about{
		position:relative;
		top:0;
		height: 100vh !important;
		background-size: cover;
		overflow: hidden;
	}

.about-info{
	/* font-family: "Montserrat"; */
  font-weight:bold;
  position: absolute;
  z-index: 100100;
  top:50%;
  color:white;
  text-align: center;
  width: 100%;
  
}
.about-info-name{
  width: 100%;
  letter-spacing: 5px;
  font-weight:800;
	/* font-size: 2.5vw; */
}

.about-info-contact{
  margin-top: 25px;
  padding-bottom: 100px;
  margin-bottom: 100px;
  height: 130px;
}


.about-info-contact   h4{
  margin-bottom: 5px;
  font-weight:500;
	/* font-size: 1.3vw; */
}

.about-info-contact p{
	font-size: 20px;
  font-weight: 300;
  margin-top: 10px;
  margin-bottom: 0
}
		
.about-info-contact a {
	margin-bottom: 5px;
  font-weight:600;
	font-size: 25px;
  /* letter-spacing: 4px; */
	color: var(--color-dark);
}

.about-content{
  float:left;
  padding-top:30px;
  background: var(--color-white);
  background-image: url("https://i.postimg.cc/GpndwV4G/1544025-ddd4c.gif");
  color:var(--color-dark);
}

/* .about-content @include respond-to(handhelds){
  padding-left:40px;
  padding-right: 40px;
} */

.about-me{
	 margin: auto; 
	text-align: justify;
	font-weight: 300;
	width: 63%;	
}
.row {
	height:100vh;
}
h1{
  z-index:-1;
  color:var(--color-dark);
  text-align:center;
  line-height: 90px;
  font-size: var(--font-xlg);
  font-weight:var(--size-ms);
  letter-spacing: -0.1em;
  width: 95%;
  margin-bottom: 10px;
  margin-top: 10px;
}

.perspective-container{
  transform:matrix(1, 0, 0, 1, 0, 0) !important
}

.photo-about {
  background: url("https://i.postimg.cc/sDjnJCtj/Meagan-2.jpg") no-repeat center center;
  background-size: cover;
  z-index: 45;
}

.hide-photo-filter {
  position: relative;
  top: 0;
  z-index: 50;
  /* width: 100%;
  height: 100%; */
}
@media screen and (max-width:620px){
  /* .photo-about{
    height:auto;
  } */
}

@media screen and (max-width: 987px) {
 h3{
  font-size: 30px;
 }
    .about-content, .about-panel {
  max-width: 100%;
  
	width: 100%;
}

/* .col-12{
  display: grid;
  grid-column: 3;
} */
.about-me{
  padding-top:670px;
  margin:20px;
  width:100%;

}
    .about-panel-wrapper{
        position: relative;
    }
}

@media screen and (max-width:1401px){
  .about-content, .about-panel{
    margin-left:0px
  }

}
</style>