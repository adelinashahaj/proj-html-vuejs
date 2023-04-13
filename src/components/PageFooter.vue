
<template>
    <footer id="site_footer">
        <div class="footer_top">
            <div class="container py-4 d-flex ">
                <div class="row-2">
                    <div class="col-3" v-for="link in menuLinks">
                        <h4>{{ link.title }}</h4>
                        <p>{{ link.text }}</p>

                        <ul>
                            <li v-for="voce in link.links" class="elemlista"><span class="freccetina">&rsaquo;</span>{{ voce }}</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer_bot py-4">
            <hr>
            <div class="container d-flex ">
                <div class="signup">
                    <p> &copy;Copyright 2012-2020 | Avada Theme by <span class="text-c">Theme Fusion</span> | All Rights Reserved |
                        Powered by <span class="text-c">WordPress</span> </p>
                </div>
                <div class="socials d-flex justify-content-end">

                    <a class="cicrcle c-4" href="#"><i class="fa-brands fa-facebook-f"></i></a>
                    <a class="cicrcle c-3" href="#"><i class="fa-brands fa-twitter"></i></a>
                    <a class="cicrcle c-2" href="#"><i class="fa-brands fa-instagram"></i></a>
                    <a class="cicrcle c-1" href="#"><i class="fa-brands fa-youtube"></i></a>


                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "PageFooter",
    data() {
        return {
            menuLinks: [
                {
                    title: "AVADA TECH FORUM",
                    text: "Send semper, nisl id feugiat eleifend, erat est digssim felis, quis auctor elit enim nec ante. Cras et nibh risus. Pellentesque non mi sit amet mi intermentum.",
                    links: []
                },
                {
                    title: "POPULAR TOPICS",
                   
                    links: [
                        " Nam a dolor volutpat massa auctor sempre",
                        " Sed euismod nunc urna fermentum arcu dapibus fringilla.",
                        " Dove Andioamo 3",
                        " Cras lacinia tellus id mauris finibus lacus molestie",
                        " curabitur a scelerisque lingua"
                    ]
                },
                {
                    title: "RECENT TOPICS",
                    links: [
                        " Cras lacinia tellus id mauris finibus lacus molestie",
                        " Proin at lingula sagittis vestibulum nisi vitae",
                        " Sed nec metus at est tincidunt elementum",
                        " Nulla egestas nulla eu nulla suscipit molestie",
                    ]
                },
                {
                    title: "LATEST REPLIES",
                    links: [
                        " Cras lacinia tellus id mauris finibus lacus molestie",
                        " Cras lacinia tellus id mauris finibus lacus molestie",
                        " Nulla egestas nulla eu nulla suscipit molestie",
                        " Mauris ec nibh quis eros sagittus lacinia a et dui",
                    ]
                }

            ]
        }

    }
}

</script>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "bootstrap";

footer {
    min-width: 60vh;

}

.footer_bot {
    z-index: 1;

    .socials {
        flex-basis: 35%;

        h3 {
            color: #0282F9;
        }

        i {
            color: white;
        }
            
        a {

        text-decoration: none;
        }
        .cicrcle {
            border-radius: 50px;
            border-radius: 50px;
            height: 40px;
            width: 40px;
            text-align: center;
            color: white;
            padding-top: 5px;
            margin-top: 30px;
            font-size: 19px;
            margin-right: 5px;

        }

        .c-1 {
            background-color: $circle1;
        }

        .c-2 {
            background-color: $circle2;
        }

        .c-3 {
            background-color: $circle3;
        }

        .c-4 {
            background-color: $circle4;
        }
    }

}

.footer_top .container {
    max-width: 1170px;
    margin: auto;

    .row-2 {
        display: flex;

        & li{
        list-style: none;
        border-bottom: 1px solid $color-bg;
        padding: 5px;
        
       }

       & h4 {
            text-transform: uppercase;
            color: black;
            font-size: 20px;
            padding-left: 28px;
            font-family: 'Fira Sans', sans-serif;
            font-weight: bold;
        }
        & h4:first-child{
            margin-bottom: 25px;
        }
        .freccetina{
            font-size: 23px;
            margin-left: -10px;
        }
        p{
            color: gray;
            padding-left: 28px;
        }

    }
    
}

.signup {
    margin-top: 35px;

    p {
        color: gray;
    }

    .text-c {
        color: black;
    }
}
</style>