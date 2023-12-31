/* General Styling Start*/
.mask {
  height: 106px;
  position: relative;
  overflow: hidden;
  margin-top: var(--offset);
}

.mask span {
  display: inline-block;
  box-sizing: border-box;
  position: absolute;
  top: 100px;
  padding-bottom: var(--offset);
  background-size: 100% 100%;
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  background-repeat: no-repeat;
}

.mask span[data-show] {
  transform: translateY(-100%);
  transition: .5s transform ease-in-out;
}

.mask span[data-up] {
  transform: translateY(-200%);
  transition: .5s transform ease-in-out;
}

.mask span:nth-child(1) {
  background-image: linear-gradient(45deg, #0ecffe 50%, #07a6f1);
}

.mask span:nth-child(2) {
  background-image: linear-gradient(45deg, #18e198 50%, #0ec15d);
}

.mask span:nth-child(3) {
  background-image: linear-gradient(45deg, #8a7cfb 50%, #633e9c);
}

.mask span:nth-child(4) {
  background-image: linear-gradient(45deg, #fa7671 50%, #f45f7f);
}
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

:root{
    --mainColor: #E1BDA5;
    --whiteColor: white;
    --titleColor: #5B745E;
    --bodyColor: #5B745E;
    --hoverColor: #5B745E;
    --backgroundColor: #5B745E;
    scroll-behavior: smooth;

}

body{
    font-family: 'Roboto', sans-serif;
    color: var(--bodyColor);
    font-weight: 400;
}

h1, h2, h3, h4{
    font-family: 'Source Sans Pro', sans-serif;
    color: var(--titleColor);
}

h1{
    font-size: 70px;
    font-weight: 700;
    color: var(--mainColor);
    text-transform: uppercase;
    margin-bottom: 10px;
    white-space: nowrap;
}

h3{
    font-size: 24px;
    font-weight: 600;
    margin-bottom: 15px;
    
}

p{
    font-size: 16px;
    line-height: 25px;
}


a{
    text-decoration: none;

}

ul{
    list-style-type: none;
}

/* general styling media query start */
@media screen and (max-width:767px) {
    h1{
    font-size: 38px;}

    h3{
        font-size: 22px;
    }

}


/* general styling media query end */
/* General Styling End */
/* Common Styling Start */

.container{
    width: 75%;
    margin: auto;
}

.clear{
    clear: both;
}

.padding{
    padding: 80px 0;
}

.section h2{
    position: relative;
    margin-bottom: 40px;
    font-size: 40px;
    font-weight: 700;
    padding-bottom: 20px;
    text-align: center;
}

.section h2::before{
    content: "";
    position: absolute;
    left: 0;
    right: 0;
    bottom: 0;
    margin: auto;
    border: var(--mainColor) solid;
    border-width: 1px 0;
    width: 70px;
    padding: 4px 0px 5px;

}

.section h2::after{
    content: "";
    position: absolute;
    left: 0;
    right: 0;
    bottom: 5px;
    background-color: var(--mainColor);
    height: 0.5px;
    width: 160px;
    margin: auto;
}

a.btn{
    color: var(--whiteColor);
}

.btn{
    display: inline-block;
    min-width: 150px;
    padding: 12px 20px;
    margin-right: 10px;
    border-radius: 4px;
    background-color: var(--mainColor);
    text-align: center;
    margin-top: 15px;
    transition: background-color 500ms;
}

.btn:hover{
    background-color: var(--hoverColor);
}

.social{
    margin-right: 15px;
    font-size: 20px;
}

a.social {
    color: var(--whiteColor);
    transition: color 500ms;
}

 a.social:hover{
    color: var(--mainColor);
}

/* Media Query of Common Styling Start */
@media screen and (max-width:1999px) {
    .container{
        width: 75%;
    }
}

@media screen and (max-width:991px) {
    .container{
        width: 90%;
    }
}

@media screen  and (max-width:767px) {
        .container{
            width: 95%;
        }

        .btn{
            min-width: 150px;
            padding: 10px 10px;
        }

        .padding{
            padding: 50px 0;
        }

        .section h2{
            font-size: 32px;
        }
    }



/* Media Query of Common Styling Start */
/* Common Styling End */
/* Navbar & Hero Section Common Styling Start*/

#home-sec{
    height: 70vh;
   
}

#home-sec .layer{
    background-color:#5B745E;
    width: 100%;
    height: 100%;
}

/* Navbar & Hero Section Common Styling End*/
/* 1. Navbar Start */

.navbar{
    position: fixed;
    top: 0;
    width: 100%;
    background-color: var(--titleColor);
    z-index: 10;
}

.nav-list li{
    display: inline-block;
}




.nav-list{
    float: right;
    width: 65%;
    text-align: right;
    padding-top: 20px;
    height: 60px;

}

.nav-list a{
    color: var(--whiteColor);
    padding: 0 7px;
    letter-spacing: 0.5px;
    font-weight: 300;
    transition: color 700ms;

}

li.active a{
    color: var(--mainColor);
    opacity: 0.9;
    
}

.nav-list a:hover{
    color: var(--mainColor);
}

.nav-menu{
    color: white;
    display: none;
    font-size: 25px;
    
}

/* Media Query of Navbar start */


@media screen and (max-width:991px){
    .nav-list{
        width: 75%;
    }

    .logo{
        width: 20%;
        margin: 0;
    }
}

@media screen and (max-width:767px){

    .nav-list ul{
        display: none;
    }
    .nav-menu{
        display: inline-block;
        margin-top: -4px;
        cursor: pointer;
    }

    .nav-list{
        float: none;
        margin-left: auto;
        text-align: right;
    }

    .logo{
        text-align: left;
        margin: 0;
    }
}
/* Media Query of Navbar end */
/* Navbar End */
/* 2. Hero Section Start */

.hero-content{
    color: var(--whiteColor);
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
}

.hero-subtitle{
    font-size: 24px;
    font-weight: 600;
}

.hero-content p{
    font-size: 26px;
    font-weight: 300;
    white-space: nowrap;
    
}

.hero-content span, .hero-content p{
    font-family: 'Source Sans Pro', sans-serif;
}

/* hero typing animation */
@keyframes typing{
    0% {
        width: 0%;
    }
    100% {
        width: 100%;
    }
    0%{
        width: 0%;
    }
}

.hero-subcontent{
    display: inline-block;
    margin-bottom: -4px;
    max-width: fit-content;
    width: 0%;
    overflow: hidden;
    border-right: 2px solid white;
    animation: typing 2s infinite alternate-reverse;
}

/* hero section media query start */

@media screen and (max-width:767px) {

    .hero-subtitle{
        font-size: 22px;
    }
    .hero-content p{
        font-size: 18px;
        font-weight: 600;
    }
    
    .hero-subcontent{
        margin-bottom: -7px;
    }
}



/* hero section media query end */
/* Hero Section End */
/* About Section Start */

.about-item{
    width: 50%;
    float: left;
}

.about-layer{
    margin: 15px;
    width: 62%;
    box-shadow: 0 0 0 8px #555555;
    border-radius: 2px;
    margin: 0 auto;
}

.overlay-inner-layer{
    position: relative;
    transform: translate(7%, 5%);
}

.about-img img{
    width: 100%;
    border-radius: 2px;
}

.social-overlay{
    position: absolute;
    background-color: rgba(0, 0, 0, 0.5);
    opacity: 0;
    width: 100%;
    height: 0%;
    bottom: 0;
    left: 0;
    transition: all 700ms;
}

.social-layer{
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);

}

.about-img:hover .social-overlay{
    opacity: 1;
    height: 100%;
    z-index: 1;
}


.about-content h2{
    position: relative;
    font-size: 34px;
    font-weight: 600;
    padding-left: 13px;
    text-transform: uppercase;
    line-height: 25px;
    margin-bottom: 30px;
}

.about-content h2::before{
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 4px;
    height: 100%;
    background-color: var(--mainColor);
    
}

.about-content .about-desc{
    border-bottom: 1px dashed var(--titleColor);
    margin-bottom: 20px;
    padding-bottom: 20px;
}

.about-content p{
font-weight: 400;
}

.about-subcontent span{
    color: var(--titleColor);
    font-weight: 500;
    
}

.about-subcontent table{
    width: 100%;
}


.about-subcontent table p{
    
    line-height: 2.5;
}

a.email-link{
    color: #7e7e7e;
}


/* about section media query start */

@media screen and (max-width:991px){
    .about-layer{
        box-shadow: none;
        width: 100%;
    } 

    .overlay-inner-layer{
        transform: none;
    }

    .about-img img, .social-overlay{
        width: 95%;
    }

    .about-subcontent table p{
        line-height: 1.7;
        font-size: 14px;
    }

    .about-content .about-desc{
        padding-bottom: 10px;
        margin-bottom: 10px;
    }


}

@media screen and (max-width:767px) {

    .about-item{
        float: none;
        width: 100%;
    }

    .about-img{
        margin-bottom: 30px;
    }

    .about-subcontent td{
        display: block;
    }
    
}

/* about section media query end */
/* About Section End */
/* our services section start */
#our-services{
    background-color: var(--backgroundColor);
    text-align: center;
}

.service-item{
    width: 25%;
    float: left;
    
}

.services-overlay{
    padding: 40px 15px;
    transition: all 500ms;
}

.service-icon{
    color: var(--mainColor);
    font-size: 30px;
    margin-bottom: 20px;
    transition: transform 500ms;
}

.services-overlay:hover{
    background-color: var(--whiteColor);
    box-shadow: 0 15px 20px rgba(0, 0, 0, 0.1);
    border-radius: 3px;
}

.service-item:hover .service-icon{
    transform: scale(1.2);
} 

/* our services media query start */

@media screen and (max-width:991px){
    .service-item{
        width: 50%;
    }

}

@media screen and (max-width:767px) {
    .service-item{
        float: none;
        width: 100%;
    }
}

/* our services media query end */
/* our services section end */
/* our portfolio section start */

#portfolio{
    text-align: center;
}

/* our portfolio section one start */


.portfolio-links a{
    display: inline-block;
    color: var(--titleColor);
    text-transform: uppercase;
    margin: 12px;
    letter-spacing: 1px;
}

.portfolio-links{
    margin-bottom: 40px;
}

.portfolio-item{
    width: 33.33%;
    float: left;
}

.portfolio-item img{
    width: 100%;
}

.portfolio-layer{
    margin: 15px;
    position: relative;
    top: 0;
    left: 0;
}

.portfolio-overlay{
    position: absolute;
    top: 0;
    left: 0;
    background-color: rgba(0, 0, 0, 0.5);
    width: 100%;
    height: 100%;
    opacity: 0; 
    transition: all 500ms;
    
}

.portfolio-overlay-content{
    position: absolute;
    right: 5%;
    bottom: 5%;
}


.portfolio-overlay-content i{
    color: var(--mainColor);
    font-size: 25px;
}

a.portfolio-active{
    color: var(--mainColor);
}

.portfolio-item:hover .portfolio-overlay{
    opacity: 1;
    z-index: 1;

}

/* our portfolio section one media query start */
@media screen and (max-width:991px){
    .portfolio-item{
        width: 50%;
    }

}


@media screen and (max-width:767px) {
    .portfolio-item{
        float: none;
        width: 100%;
    }

    .portfolio-item:not(:last-of-type){
        margin-bottom: 35px;
    }
}


/* our portfolio section one media query end */
/* our portfolio section one end */
/* our portfolio section two start */

.portfolio-sec2{
    background-color: var(--backgroundColor);
}

.portfolio-numbers{
    width: 25%;
    float: left;
}

.portfolio-numbers-layer{
    margin: 10px;
    
}

.portfolio-numbers h3{
    font-weight: 800;
    font-size: 26px;
}

.portfolio-numbers span{
    font-weight: 600;
    font-family: 'Source Sans Pro', sans-serif;

}

.portfolio-numbers i{
    color: var(--mainColor);
    font-size: 26px;
    margin-bottom: 15px;
}


/* our portfolio section one media query start */

@media screen and (max-width:767px) {
    .portfolio-numbers{
        float: none;
        width: 100%;
    }

    .portfolio-numbers:not(:last-of-type){
        margin-bottom: 30px;
    }
}


/* our portfolio section one media query end */

/* our portfolio section two end */
/* our portfolio section end */
/* testimonials section start */

.feedback-card{
    background-color: var(--backgroundColor);
    width: 70%;
    margin: auto;
    padding: 40px;
    position: relative;
    overflow: hidden;
}

.feedback-item{
    float: left;
}

.feedback-img{
    width: 18%;
    position: relative;
    z-index: 2;
}

.feedback-card::before{
    content: "";
    position: absolute;
    background-color: var(--mainColor);
    top: -37%;
    left: -10%;
    width: 24%;
    height: 100%;
    transform: rotate(42deg);
    
}

.feedback-content{
    width: 80%;
}

.feedback-img img{
    width: 100%;
    border-radius: 50%;

}

.testimonial-layer{
    margin-right: 20px;
}

.feedback-content a{
    display: inline-block;
    color: #777777;
    font-size: 15px;
    font-weight: 600;
    margin-bottom: 10px;
    font-family: 'Source Sans Pro', sans-serif;
}

.feedback-content p{
    font-style: italic;
    margin-bottom: 20px;
}

.feedback-content .fa-star{
    color: #f1c30d;
}

.feedback-slider-icon{
    text-align: center;
    margin-top: 10px;
    cursor:default;
}

.active-icon{
    display: inline-block;
    background-color: var(--mainColor);
    border-radius: 10px;
    padding: 5px 12px 6px 13px;
}

.disabled-icon{
    display: inline-block;
    border: solid 1px var(--mainColor);
    width: 12px;
    height: 12px;
    border-radius: 50%;
    
}

.active-icon, .disabled-icon{
    cursor: pointer;
}


/* testimonial section media query start */
@media screen and (max-width:991px){
    .feedback-card{
        width: 100%;
        padding: 40px;
    }

    .feedback-img{
        width: 20%;
    }
}


@media screen and (max-width:767px) {
    .feedback-card{
        width: 100%;
        padding: 20px;
    }

    .feedback-card::before{
        top: -37%;
        left: -10%;
        width: 35%;
    }

    .feedback-img{
        width: 35%;
        left: 50%;
        transform: translateX(-50%);
        margin-bottom: 40px;
    }
    .feedback-content{
        width: 100%;
    }
}
/* testimonial section media query end */
/* testimonials section end */
/* blog section start */
#blog{
    background-color: var(--backgroundColor);
}

.blogs{
    overflow: auto;
}

.blog-item{
    width: 33.33%;
    float: left;
}

.blog-item img{
    width: 100%;
}

.blog-video{
    position: relative;
    aspect-ratio: 16/9;

}

.blog-video iframe{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

.blog-layer{
    margin: 15px;
    background-color: var(--whiteColor);
}

.blog-meta{
    display: inline-block;
    margin-bottom: 10px;
    font-size: 15px;
}

.blog-content{
    padding: 20px;
}

.blog-content p{
    margin-bottom: 20px;
}

.read-more-link{
   color: var(--titleColor);
   text-transform: uppercase;
   transition: color 500ms;
    
}

.blog-title a{
    color: var(--titleColor);
    transition: color 500ms;
}

.blog-title a:hover, .read-more-link:hover{
    color: var(--mainColor);
}

/* Media Query of blog section start */
@media screen and (max-width:1999px){
    .blog-content{
        min-height: 320px;

    }
}


@media screen and (max-width:991px){

    .blog-content{
        min-height: 350px;
        padding: 10px;

    }
    .blog-title a{
        font-size: 19px;
    }
}

@media screen and (max-width:767px) {
    .blog-item{
        width: 100%;
        float: none;
    }

    .blog-item:not(:last-of-type){
        margin-bottom: 30px;
    }
        .blog-content{
        min-height: 250px;

    }
}


/* Media Query of Blog Section end */
/* blog section end */
/* contact section start */
.contact-form{
    margin: auto;
    width: 80%;
    padding: 40px;
}

.full-name, .email{
    width: 50%;
    float: left;
}

form{
    overflow: auto;
}

.contact-form input, textarea{
    width: 100%;
    padding: 12px;
    border-radius: 4px;
    margin-bottom: 30px;
    box-shadow: inset 0 1px 1px rgba(0,0,0,.075);
    border: 1px solid #ccc;
    font-family: 'Roboto', sans-serif;
    font-size: 14px;
    color: lightgray;
    font-weight: 400;
    
}

.contact-form input:focus, textarea:focus{
    border-color: var(--mainColor);
    color: black;
    outline: none;
}

.input-layer{
    margin: 0 15px;
}

.contact-form textarea{
    resize: vertical;
    height: 100px;
}

.form-submit button{
    color: white;
    border: none;
    text-transform: uppercase;
    font-size: 14px;
    font-weight: 400;
    margin-top: 0;
    cursor:not-allowed;
}


/* Media Query of contact section start */
@media screen and (max-width:991px){
    .contact-form{
        width: 100%;
        padding: 0;
    }

    .contact-form input, textarea{
        margin-bottom: 25px;
    }
}

@media screen and (max-width:767px) {
    .contact-form{
        width: 100%;
        padding: 0;
    }

    .full-name, .email{
        width: 100%;
        float: none;
    }

    .contact-form input, textarea{
        margin-bottom: 20px;
    }
}

/* Media Query of contact section end */
/* contact section end */
/* footer section start */

#footer{
    background-color: var(--titleColor);
    padding: 60px 0px;
    text-align: center;
}

.footer-social-icons a{
    display: inline-block;
    margin-bottom: 15px;
    font-size: 14px;
}


#footer p{
    color: white;
}

#footer .copyrights{
    color: var(--mainColor);
}

#footer .copyrights:hover{
    text-decoration: underline;
}
/* footer section end */
