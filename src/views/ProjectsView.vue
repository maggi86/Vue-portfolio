<template>
    <div class="container">
		<div class="box">
			<div class="thumb">
				<img src="https://i.postimg.cc/C1Xn4HS3/Screenshot-2022-05-11-115811.png">
			</div>
			<div class="details">
				<div class="content">
					<h3>Swamp</h3>
					<a href="https://github.com/maggi86/nav-example"><i class="bi bi-github"></i>
                    </a>
					<a href="https://swamp-stardust-fc706b.netlify.app/"><span class="iconify" data-icon="file-icons:netlify"></span>
                    </a>
				</div>
			</div>
		</div>
		<div class="box">
			<div class="thumb">
				<img src="https://i.postimg.cc/cJKscqCJ/Screenshot-2022-07-21-101213.png">
			</div>
			<div class="details">
				<div class="content">
					<h3>BMI Calculator</h3>
					<a href="https://github.com/maggi86/BMI-calculator"><i class="bi bi-github"></i>
                    </a>
					<a href="https://graceful-crisp-3d45ef.netlify.app/"><span class="iconify" data-icon="file-icons:netlify"></span>
                    </a>
				</div>
			</div>
		</div>
		<div class="box">
			<div class="thumb">
				<img src="https://i.postimg.cc/8z782RSK/Screenshot-2022-07-21-110835.png">
			</div>
			<div class="details">
				<div class="content">
					<h3>Anime Boys Website</h3>
					<a href="https://github.com/maggi86/PropertyList"><i class="bi bi-github"></i>
                    </a>
					<a href="https://property-anime-boys.netlify.app/"><span class="iconify" data-icon="file-icons:netlify"></span>
                    </a>
				</div>
			</div>
		</div>
		<div class="box">
			<div class="thumb">
				<img src="https://i.postimg.cc/XJCdmDHj/Screenshot-2022-07-21-111110.png">
			</div>
			<div class="details">
				<div class="content">
					<h3>Wig Nation</h3>
					<a href="https://github.com/maggi86/wigs"><i class="bi bi-github"></i>
                    </a>
					<a href="#"><span class="iconify" data-icon="file-icons:netlify"></span>
                    </a>
				</div>
			</div>
		</div>
		<div class="box">
			<div class="thumb">
				<img src="https://i.postimg.cc/ydX8BZD2/Screenshot-2022-07-21-161544.png">
			</div>
			<div class="details">
				<div class="content">
					<h3>To Do List</h3>
					<a href="https://github.com/maggi86/toDoList"><i class="bi bi-github"></i>
                    </a>
					<a href="https://euphonious-puffpuff-e5c779.netlify.app/"><span class="iconify" data-icon="file-icons:netlify"></span>
                    </a>
				</div>
			</div>
		</div>
		<div class="box">
			<div class="thumb">
				<img src="https://i.postimg.cc/yxHngwYk/Screenshot-2022-07-21-161915.png">
			</div>
			<div class="details">
				<div class="content">
					<h3>Hex to RGB</h3>
					<a href="https://github.com/maggi86/hextoRGB"><i class="bi bi-github"></i>
                    </a>
					<a href="https://sweet-chaja-308937.netlify.app/"><span class="iconify" data-icon="file-icons:netlify"></span>
                    </a>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
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
	width: 80%;
	margin-top: 130px;
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
	box-shadow: 0 5px 20px rgba(0,0,0,1);
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
	background: #262626;
}

.container .box:nth-child(1) .details {
	background: var(--color-gray);
}

.container .box:nth-child(2) .details {
	background: var(--color-dark);
}

.container .box:nth-child(3) .details {
	background: var(--color-gray);
}

.container .box:nth-child(4) .details {
	background: var(--color-dark);
}
.container .box:nth-child(5) .details {
	background: var(--color-gray);
}

.container .box:nth-child(6) .details {
	background: var(--color-dark);
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
	color: #262626;
	background: rgb(200, 12, 12);
}

/*media queries */
@media (max-width: 1000px) {
	.container {
		width: 100%;
		height: auto;
		padding: 20px;
		box-sizing: border-box;
	}

	.container .box {
		height: 250px;
	}

	.container .box .thumb {
		display: none;
	}
}

@media (max-width: 768px) {
	.container {
		display: initial;
	}

	.container .box {
		width: 50%;
		height: 250px;
		float: left;
	}
}

@media (max-width: 480px) {
	.container {
		top: 0;
		left: 0;
		transform: translate(0);
		/*padding: 10px;*/
	}

	.container .box {
		width: 100%;
		height: 250px;
		float: none;
	}
}
</style>