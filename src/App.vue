<template> 
<body>
  <Navbar/>

<main>
  <router-view />
</main>
<foot />
</body>  

</template>

<script>
// @ is an alias to /src
import Navbar from "./components/navbar.vue";
import foot from "@/components/footer.vue";

export default {
  components: {
    Navbar,
    foot
},
};
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
body{
  background-color: var(--color-white);
}
main{
  margin-left: 250px;
}
</style>


