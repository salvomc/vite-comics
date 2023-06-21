<script>
export default {
    data() {
        return {

                navLinks:
                    [
                        {
                            section_name : 'digital comics',
                            section_icon : './src/assets/buy-comics-digital-comics.png',
                            active: false,
                            link:'#'
                        },
                        {
                            section_name : 'dc merchandise',
                            section_icon : './src/assets/buy-comics-merchandise.png',
                            active: false,
                            link:'#'
                        },
                        {
                            section_name : 'subscription',
                            section_icon : './src/assets/buy-comics-subscriptions.png',
                            active: false,
                            link:'#'
                        },
                        {
                            section_name : 'comic shop locator',
                            section_icon : './src/assets/buy-comics-shop-locator.png',
                            active: false,
                            link:'#'
                        },
                        {
                            section_name : 'dc power visa',
                            section_icon : './src/assets/buy-dc-power-visa.svg',
                            active: false,
                            link:'#'
                        },
                    ]
            }
        },
}
</script>

<template>
    <footer>
        <div class="navbar-container">
            <ul>
                <li v-for="(navLink, index) in navLinks" :key="index">
                    <a :href="navLink.link">
                        <img :src="navLink.section_icon" alt="">
                        <span> {{navLink.section_name.toUpperCase()}}</span>
                    </a>
                </li>
            </ul>
        </div>
        <div class="dc-logo-footer">
            <div class="link-list-container">
                <div class="link-list">
                    <ul>
                        <li>
                            <h5>DC COMICS</h5>
                        </li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                        <li>
                            <h5>SHOP</h5>
                        </li>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                    <ul>
                        <li>
                            <h5>DC</h5>
                        </li>
                        <li>Term Of Use</li>
                        <li>Privacy Policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                    <ul>
                        <li>
                            <h5>SITES</h5>
                        </li>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </div>
        </div>
        <section class="bottom-footer">
            <div class="link-list-container">
                <a href="#">SIGN-UP NOW!</a>
                <div class="link-social">
                    <h4>FOLLOW US</h4>
                    <a href="#" class=""><img src="/img/footer-facebook.png" alt="Facebook"></a>
                    <a href="#" class=""><img src="/img/footer-twitter.png" alt="Twitter"></a>
                    <a href="#" class=""><img src="/img/footer-youtube.png" alt="YouTube"></a>
                    <a href="#" class=""><img src="/img/footer-pinterest.png" alt="Pinterest"></a>
                    <a href="#" class=""><img src="/img/footer-periscope.png" alt="Periscope"></a>
                </div>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/generals' as *;



</style>