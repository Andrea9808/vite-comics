<script>

export default {
    name: "FooterSection",

}

</script>

<template>
    <div class="bg">

        <div class="container">

            <div class="navbar_footer">

                <div class="link">
                    <h5>DC COMICS</h5>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <h5>SHOP</h5>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collections</a></li>
                    </ul>
                </div>

                <div class="link">
                    <h5>DC</h5>
                    <ul>
                        <li><a href="#">Terms of Use</a></li>
                        <li><a href="#">Privacy Policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>


                <div class="link">
                    <h5>SITES</h5>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>
            </div>






            <div class="logo_bg">
                
            </div>
        </div>

    </div>
</template>




<style lang = 'scss' scoped>
@use '../Styles/partials/_variables.scss' as *;
@use '../Styles/partials/mixins' as *;


.bg {
    background-image: url('/public/img/footer-bg.jpg');



    h5 {
        color: white;
        font-size: 15px;
        padding: 10px 0;
        margin-bottom: 10px;
    }

    a {
        color: gray;
        font-size: 12px;
        text-decoration: none;

        &:hover {
            text-decoration: underline;
        }
    }

    li {
        list-style-type: none;
    }


}

.logo_bg{
    background-image: url(public/img/dc-logo-bg.png);
    width: 30%;
    background-size: cover;
    background-position: center;
}

.container {
    display: flex;
    justify-content: space-between;
    max-width: 1170px;
    margin: auto;


    .navbar_footer {
        margin-top: 20px;
        display: flex;
    }

    .link{
        margin-right: 20px;
    }
}
</style>
