<template>
<div class="container">
        <aside class="container-aside">
            <div class="containerAside-header">
                <div class="asideHeader-userInformations">
                <img src="https://i.postimg.cc/sDjnJCtj/Meagan-2.jpg" class="asideHeader-imgUserImage">
                  <h3 class="asideHeader-lblUserName"><span class="caps">M</span>eagan <span class="caps">W</span>illiams</h3>
                    <div class="asideHeader-socialsBox">
                        <a href="https://github.com/maggi86" class="asideHeader-btnSocial"><i class="bi bi-github"></i></a>
                        <a href="https://www.linkedin.com/in/meagan-williams-087920238/" class="asideHeader-btnSocial"><i class="bi bi-linkedin"></i></a>
                    </div>
                </div>
            </div>
            <div class="containerAside-main">
                <div class="asideMain-menuItemsBox">
                    <div class="asideMain-menuItem">
                          <a href="/" class="mainMenu-btnMenuItem"><i class="bi bi-house"></i> <span
                          class="mainMenu-lblMenuItem">Home</span></a>
                    </div>
                    <div class="asideMain-menuItem">
                        <a href="about" class="mainMenu-btnMenuItem"><i class="bi-person"></i> <span
                        class="mainMenu-lblMenuItem">About</span></a>
                    </div>
                    <div class="asideMain-menuItem">
                        <a href="resume" class="mainMenu-btnMenuItem"><i class="bi bi-file-earmark"></i> <span
                        class="mainMenu-lblMenuItem">Resume</span></a>
                    </div>
                    <div class="asideMain-menuItem">
                        <a href="projects" class="mainMenu-btnMenuItem"><i class="bi bi-book"></i> <span
                        class="mainMenu-lblMenuItem">Projects</span></a>
                    </div>
                    <div class="asideMain-menuItem">
                        <a href="contact" class="mainMenu-btnMenuItem"><i class="bi bi-envelope"></i> <span
                        class="mainMenu-lblMenuItem">Contacts</span></a>
                    </div>
                    <div class="asideMain-menuItem">
                        <a href="testimonial" class="mainMenu-btnMenuItem"><i class="bi bi-chat-left-quote"></i> <span
                        class="mainMenu-lblMenuItem">Testimonial</span></a>
                    </div>
                </div>
            </div>
        </aside>
        <div>
            <button @click="ShowMenu()" class="containerMain-ShowMenu"><i class="bi bi-list"></i></button>
        </div>   
      </div>
</template>


<script>

export default{
    methods: {
        ShowMenu() {
    let menu = document.querySelector(".container-aside"),
        btnShowMenu = document.querySelector(".containerMain-ShowMenu");
    menu.classList.toggle("showMenu");
    if (btnShowMenu.innerHTML == "<i class=\"bi bi-list\"></i>")
        btnShowMenu.innerHTML = "<i class=\"bi bi-x-lg\"></i>";
    else
        btnShowMenu.innerHTML = "<i class=\"bi bi-list\"></i>";
        btnShowMenu.innerHTML = "<i class=\"bi bi-x-lg\"></i>";
            },
scrollFunction() {
  if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
    document.getElementById("navbar").style.top = "0";
  } else {
    document.getElementById("navbar").style.top = "-50px";
  }
}
    }
}
</script>


<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans&family=Poppins:wght@400;600&family=Raleway:wght@700&display=swap');
/* * {
    font-family: 'Raleway', sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
} */

:root {
    --color-primary: #ef1e48;
    --color-white: #e8e6e3;
    --color-black: #030910;
    --color-dark: #642330;
    --color-gray: #9d8790;


    --font-Poppins: 'Poppins', sans-serif;
    --font-Raleway: 'Raleway', sans-serif;
    --font-OpenSans: 'Open Sans', sans-serif;

    --font-lg: 64px;
    --font-md: 26px;
    --font-sm: 15px;
    --font-xs: 9px;

    --size-lg: 1280px;
    --size-md: 976px;
    --size-sm: 768px;
    --size-xs: 500px;
}

html, body {
    height: 100%;
}

a {
    text-decoration: none;
}
.caps{
    font-size:30px
}
div.container {
    width: 100%;
    height: 100%;

}

.container-aside {
    width: 12%;
    overflow-y: auto;
overflow-x:hidden ;
    max-width: 300px;
    min-width: 250px;
    height: 100%;
    position: fixed;
    left: 0;
    top: 0;
    z-index: 4;
    /* font-size: 30px; */
    background-color: var(--color-black);
    transition: left 1s;
}

.showMenu {
    left: 0 !important;
}
/* span{
    font-size:20px;
    font-weight:600;
    margin-left:1 0px;
    letter-spacing:1.7px;
} */

h3{
    font-size:18px;
    font-weight:600;
    /* letter-spacing:1.7px; */
}
.containerMain-ShowMenu {
    display: none;
    position: fixed;
    top: 10px;
    right: 10px;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    z-index: 5;
    border: none;
    /* font-family: var(--font-OpenSans); */
    font-size: var(--font-md);
    /* background-color: var(--color-white); */
    color: var(--color-white);
    cursor: pointer;
} 

.container-aside, .asideHeader-userInformations {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 20px 0;    
}

.asideHeader-imgUserImage {
    width: 120px;
    height: 120px;
    border-radius: 50%;
    border: 4px solid #000000;
    margin-bottom: 20px;
}

.asideHeader-lblUserName {
    /* font-family: var(--font-Poppins); */
    font-size: var(--font-md);
    font-weight: 500;
    font-size:25px;
    color: white;
    margin-bottom: 20px;
}

.asideHeader-btnSocial {
    padding: 10px 12px;
    margin: 0 2px;
    border-radius: 50%;
    background-color: var(--color-dark);
    color: var(--color-white);
    font-size: var(--font-sm);
    transition: background-color .5s;
}

.asideHeader-btnSocial:hover {
    background-color: var(--color-primary);
}

.mainMenu-btnMenuItem {
    color: var(--color-gray);
    /* font-family: var(--font-OpenSans); */
    font-size: var(--font-sm);
    font-weight: 500;
    font-size:20px;
    line-height:53px;
    /* letter-spacing:3px; */
    transition: color .5s;
}

@media screen and (max-width: 1400px) {
    .container-aside {
        left: -100%;
    }
    
    
    .containerMain-ShowMenu {
        display: block;
        background-color:var(--color-dark);
    }

    /* .containerMain-lblName, .containerMain-lblAbility {
        margin-left: 10vw;
    } */
}

</style>