<template>
	<h2 class="text-center py-5">Projects</h2>
	<section>
    <div class="container mb-5" id="project">
        <!-- <div class="row mx-auto"> -->
            <!-- <div class="col-md-12"> -->
                
                <div class="box" v-for="project in projects">
                <div class="thumb">
                    <img :src="project.image">
                </div>
                <div class="details">
                    <div class="content">
                        <h3>{{project.name}}</h3>
                        <a :href="project.github"><i class="bi bi-github"></i>
                        </a>
                        <a :href="project.netlify"><span class="iconify" data-icon="file-icons:netlify"></span>
                        </a>
                    </div>
                    </div>
                <!-- </div> -->
            <!-- </div> -->
        </div>
    </div>
    
		<!-- <div class="box">
			<div class="thumb">
				<img href="{{project.image[1]}}">
			</div>
			<div class="details">
				<div class="content">
					<h3>{{project.name[1]}}</h3>
					<a href="{{project.github[1]}}"><i class="bi bi-github"></i>
                    </a>
					<a href="{{project.netlify[1]}}"><span class="iconify" data-icon="file-icons:netlify"></span>
                    </a>
				</div>
			</div>
		</div>
		<div class="box">
			<div class="thumb">
				<img href="{{project.image[2]}}">
			</div>
			<div class="details">
				<div class="content">
					<h3>{{project.name[2]}}</h3>
					<a href="{{project.github[2]}}"><i class="bi bi-github"></i>
                    </a>
					<a href="{{project.netlify[2]}}"><span class="iconify" data-icon="file-icons:netlify"></span>
                    </a>
				</div>
			</div>
		</div> -->
	<!-- </div>
	<div class="container mb-5">
		<div class="box">
			<div class="thumb">
				<img href="{{project.image[3]}}">
			</div>
			<div class="details">
				<div class="content">
					<h3>{{project.name[3]}}</h3>
					<a href="{{project.github[3]}}"><i class="bi bi-github"></i>
                    </a>
					<a href="{{project.netlify[3]}}"><span class="iconify" data-icon="file-icons:netlify"></span>
                    </a>
				</div>
			</div>
		</div>
		<div class="box">
			<div class="thumb">
				<img href="{{project.image[4]}}">
			</div>
			<div class="details">
				<div class="content">
					<h3>{{project.name[4]}}</h3>
					<a href="{{project.github[4]}}"><i class="bi bi-github"></i>
                    </a>
					<a href="{{project.netlify[4]}}"><span class="iconify" data-icon="file-icons:netlify"></span>
                    </a>
				</div>
			</div>
		</div>
		<div class="box">
			<div class="thumb">
				<img href="{{project.image[5]}}">
			</div>
			<div class="details">
				<div class="content">
					<h3>{{project.name[5]}}</h3>
					<a href="{{project.github[5]}}"><i class="bi bi-github"></i>
                    </a>
					<a href="{{project.netlify[5]}}"><span class="iconify" data-icon="file-icons:netlify"></span>
                    </a>
				</div>
			</div>
		</div>
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
	justify-content: center;
    margin-bottom: 300px;
}
.box{
	 margin: 5px; 
}
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

body {
	background: var(--color-gray);
	margin: 0;
	padding: 0;
	font-family: sans-serif;
}

.container {
	/* position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%); */
	display: flex;
	width: 100%;
    margin-bottom: 59px;
	/* margin-bottom: 130px; */
	/*width: 1000px;*/
	/* height: 500px; */
}

.container .box {
	position: relative;
	width: 250px;
	height: 360px;
	background: var(--color-gray); 
	transition: 0.5s;
}

.container .box:hover {
	transform: scale(1.1);
	z-index: 1;
	box-shadow: 0 5px 20px var(--color-dark);
}

.container .box .thumb,
.container .box .details {
	position: absolute;
	width: 100%;
	height: 180px;
	overflow: hidden;
}

.container .box:nth-child(odd) .thumb,
.container .box:nth-child(even) .details  {
	bottom: 0;
	left: 0;
}

.container .box .thumb img {
	width: 100%;
	height: 100%;
}

.container .box .details {
	background: var(--color-dark);
}

.container .box:nth-child(1) .details {
	background: var(--color-gray);
}

.container .box:nth-child(3) .details {
	background: var(--color-gray);
}

.container .box:nth-child(5) .details {
	background: var(--color-gray);
}

.container .box .details .content {
	position: absolute;
	top: calc(50% + 16px);
	transform: translateY(-50%);
	width: 100%;
	padding: 20px;
	text-align: center;
	transition: 0.5s;
	box-sizing: border-box;
}

.container .box:hover .details .content {
	top: calc(50%);
}

.container .box .details .content .fas {
	font-size: 70px;
	color: var(--color-black);
}

.container .box .details .content h3 {
	margin: 0;
	padding: 10px 0;
	color: var(--color-black);
}

.container .box .details .content a {
	display: inline-block;
	padding: 5px 20px;
	color: rgb(6, 5, 5);
	border: 2px solid var(--color-black);
	text-decoration: none;
	transition: 0.5s;
	border-radius: 20px;
	transform: scale(0);
}

.container .box:hover .details .content a {
	transform: scale(1);
}

.container .box .details .content a:hover {
	color: #ffffff;
	background: rgb(0, 0, 0);
}

/*media queries */
@media (max-width: 900px) {
	.container .box{
        position: relative;
    }
}
</style>