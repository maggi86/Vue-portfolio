<template>
<section>
	<h1 class="text-center py-5 mb-5">Projects</h1>
	<a class="container" id="project">
	
    
        <!-- <div class="row mx-auto"> -->
            <!-- <div class="col-md-12"> -->	
                
                 <div class="row" > 
                <div class="col mx-auto" v-for="project in projects" :key="project"> 
					<div class="card" :href="project.netlify" >

						<div class="img">
                    <img :src="project.image">
                        </div>
                <div class="details">
                    <div class="content">
                        <h3>{{project.name}}</h3>
                        <a :href="project.github"><i class="bi bi-github"></i>
                        </a>
                    </div>
                </div>
			</div>
			</div>
                </div>
            </a>
        <!-- </div>
    </div> -->

	</section>
</template>

<script>
export default{
    computed:{
        projects(){
          return this.$store.state.project;
        }
}
}
</script>

<style scoped>
.container{
	/* justify-content: center; */
    padding-left: 260px;
}
.card{
	width: 240px;
	height: 320px;
	 margin: 5px; 
}
/* .col{
	width:300px
} */
:root {
    --color-primary: #ef1e48;
	---color-white: #aba8a482;
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
	
	margin: 0;
	padding: 0;
	/* font-family: sans-serif; */
}
img{
	height:250px;
	width:240px
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
section{
background: var(--color-white);
	background-image: url("https://i.postimg.cc/GpndwV4G/1544025-ddd4c.gif");
}
.container {
	/* position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%); */
	display: flex;
	width: 100%;
    padding-bottom: 59px;
	
	/* margin-bottom: 130px; */
	/* width: 1000px; */
	/* height: 500px; */
}

.container .card {
	position: relative;
	
	background: var(--color-gray); 
	transition: 0.5s;
}

.container .card:hover {
	transform: scale(1.1);
	z-index: 1;
	box-shadow: 0 5px 20px var(--color-dark);
}

.container .card .img,
.container .card .details {
	position: absolute;
	width: 100%;
	height: 140px;
	overflow: hidden;
}


.container .card .thumb img {
	width: 100%;
	height: 100%;
}

.container .card .details {
	background: var(--color-dark);
}


.container .card .details .content {
	position: absolute;
	top: calc(50% + 16px);
	transform: translateY(-50%);
	width: 100%;
	padding: 20px;
	text-align: center;
	transition: 0.5s;
	/* box-sizing: border-box; */
}

.container .card:hover .details .content {
	top: calc(50%);
}

.container .card .details .content .fas {
	font-size: 70px;
	color: var(--color-black);
}

.container .card .details .content h3 {
	margin: 0;
	padding: 10px 0;
	color: var(--color-black);
}

.container .card .details .content a {
	display: inline-block;
	padding: 5px 20px;
	color: rgb(0, 0, 0);
	border: 1px solid var(--color-black);
	text-decoration: none;
	transition: 0.5s;
	border-radius: 20px;
	transform: scale(0);
}

.container .card:hover .details .content a {
	transform: scale(1);
}

.container .card .details .content a:hover {
	color: #ffffff;
	background: rgb(0, 0, 0);
}

/*media queries */
@media (max-width: 992px) {
	.container {
		padding-left:10%;
	}
}
@media screen and (max-width:1400px){
.container{
	padding-left:3%;
}
}
@media screen and (max-width:1300px){
	.container{
		display:grid;
		padding-left: 60px;
	}
	img{
	height:200px;
	width:250px
}
.container .card .img,
.container .card .details {
	height: 200px;

	

}
.card{
	height: 380px;
	width: 250px
}
}
</style>