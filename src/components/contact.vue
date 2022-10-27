<template>

    <body>
        <section class="contact" id="contact">
            <div class="container  mx-auto text-center d-flex justify-content-center">
                <div class="row">
                    <div class="col-md-12">
                        <div class="heading text-center">
                            <h1>Contact
                                <span> Me </span>
                            </h1>
                            <p>I'd love to hear from you!
                                FEEL FREE TO CONTACT ME! </p>
                            <!-- <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                        <br>incididunt ut labore et dolore magna aliqua.</p> -->
                        </div>
                    </div>
                    <div class="col">
                        <div class="title">
                            <h2>Contact detail</h2>

                        </div>
                        <div class="content">
                        <div class="row">

                            <div class="info">
                                <i class="bi bi-telephone"></i>
                                <h4 class="d-inline-block ms-5 ps-3">PHONE :
                                    <br>
                                    <span>+27 67 155 0947
                                        <br>+27 81 496 3622</span>
                                </h4>
                            </div></div>
                        
                            <div class="row">
                            <div class="info">
                                <i class="bi bi-envelope"></i>
                                <h4 class="d-inline-block">EMAIL :
                                    <br>
                                    <span>meaganwilliams407@gmail.com</span>
                                </h4>
                            </div>
                        </div>
                    </div>
                    </div>
                    <div id="Forrm" class="col">
                        <form action="https://formspree.io/f/xayvrnkd" method="POST">
                            <div class="row me-4">

                                <input type="text" class="form-control" placeholder="Name" name="fname" required>

                                <input type="email" class="form-control" placeholder="Email" name="email" required>


                                <input type="text" class="form-control" placeholder="Subject" name="subject" required>

                                <div class="form-group">
                                    <textarea class="form-control" rows="5" id="comment"
                                        placeholder="Message"></textarea>
                                </div>
                            </div>
                            <!-- <div class="form-group">
                            <textarea class="form-control" rows="5" id="comment" placeholder="Message"></textarea>
                        </div> -->
                            <button class="btn btn-block" type="submit">Send Now!</button>
                        </form>
                    </div>
                </div>
            </div>
        </section>
    </body>
</template>

<script>
// import Foot from "@/components/footer.vue";

export default {
    data() {
        return {
            name: "",
            email: "",
        }
    },

};
</script>

<style scoped>
body {
    background-color: var(--color-white);
    width: 100%;
    max-width: 100%;
    padding-bottom: 70px;
    background-image: url("https://i.postimg.cc/GpndwV4G/1544025-ddd4c.gif");
}

.title {
    padding-top: 40px;
}

section {
    margin-right: 30px;
    margin-left: 30px;

}

* {

    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

:root {
    --color-primary: #ef1e48;
    --color-white: #aba8a482;
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
    --size-mi: 300px;
}

.contact {
    padding: 50px 0;
}

.contact .heading h2 {
    font-size: var(--font-md);
    font-weight: var(--size-sm);
    margin: 0;
    padding: 0;

}

.contact .heading h2 span {
    color: var(--color-primary)
}

.contact .heading h1{
    color: var(--color-dark);
    margin: 10px 50px 20px;
  z-index:-1;
  color:var(--color-dark);
  text-align:center;
  line-height: 90px;
  font-size: var(--font-lg);
  font-weight:var(--size-ms);
  letter-spacing: 0em;
  width: 95%;
  /* margin-bottom: 10px; */
  /* margin-top: 10px; */
}
.contact .form-control {
    padding: 25px;
    font-size: var(--font-sm);
    margin-bottom: 10px;
    margin: 10px;
    background: rgb(230, 230, 230);
    border: 0;
    border-radius: 10px;
}

.contact button.btn {
    padding: 10px;
    border-radius: 10px;
    font-size: var(--font-sm);
    background: var(--color-gray);
    color:rgb(78, 76, 76);
}

.contact .title h3 {
    font-size: var(--font-sm);
    font-weight: var(--size-md);
}

.contact .title p {
    font-size: var(--font-sm);
    font-weight: var(--size-xs);
    color: var(--color-gray);
    line-height: 1.6;
    margin: 0 0 40px;
}

.contact .content .info {
    margin-top: 30px;
    display:inline-flex;
}
i {
    display:block;
}
.contact .content .info i {
    font-size: var(--font-md);
    padding: 0;
    margin: 0;
    color: var(--color-black);
    margin-right: 20px;
    margin-left:200px;
    text-align: center;
    width: 20px;
}
    .contact .title {
        margin-left:150px
    }
.contact .content .info h4 {
    /* font-size: var(--font-sm); */
    line-height: 1.4;
}

.contact .content .info h4 span {
    font-size: var(--font-sm);
    font-weight: var(--size-mi);
    color: rgb(78, 76, 76);
}

.btn {
    margin-left: 10px;
}
@media screen and (max-width:1200px){
    .contact .content .info i {
        margin-left:130px
    }
    .contact .title {
        margin-left:0
    }
}

@media screen and (max-width:992px){
    .contact .content .info i {
        margin-left:0px
    }
}
</style>
