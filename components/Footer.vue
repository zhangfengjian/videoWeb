<template>
    <div class="footer-wrap">
        <footer>
            <p class="allright"> © 2018 All Rights Reserved.</p>
            <div class="allright">
                <ul class="site-links">
                    <li><a href="#">Home</a></li>
                    <li><a href="#">About Us</a></li>
                    <li><a href="#">Faq</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
            </div>
        </footer>
    </div>
</template>
<style lang="scss">
.footer-wrap{
    background: #2e2e2e;
    color: #fff;
    padding: 30px 0;
    border-top: 5px solid #EC5538;
    .allright{
        text-align: center;
        margin-bottom: 0;
    }
    .site-links{
        list-style: none;
        padding: 0;
        margin: 0;
        li{
            display: inline-block;
            margin-right:5px;
        }
        a{
            color: #fff;
        }
    }
}
</style>