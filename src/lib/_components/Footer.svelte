<script lang='ts'>

</script>

<div class="Footer uk-flex uk-flex-between uk-width-1-1 ">
    <div class="FooterContainer uk-flex uk-flex-column uk-flex-center uk-flex-top uk-width-1-5 uk-visible@m">
        <a href="https://abiferguson.glossgenius.com/services" target="_blank" class="externalLink">Book An Appointment</a>
        <a href="https://goldielocks.com/?sca_ref=2599066.5T9VJPRpfc&utm_medium=uppromote&utm_source=affiliates" target="_blank" class="externalLink">Shop Custom Hair Care</a>
        <a href="https://www.invisiblebeadextensions.com/blog/all-about-ibe/" target="_blank" class="externalLink">Learn More About IBE®</a>
    </div>

    <div class="FooterContainer uk-flex uk-flex-column uk-flex-center uk-flex-top uk-width-1-5 uk-width-1-5">
        <a href="https://maps.app.goo.gl/r5W8J5yNyjKDiEo59" target="_blank" class="externalLink">3725 Broadway Blvd Suite 204, Kansas City, MO 64111</a>
        <p>By Appointment Tuesday - Sunday </p>
    </div>

    <div class="FooterContainer uk-flex uk-flex-column uk-flex-center uk-flex-top uk-width-1-5 uk-width-1-5">
        <a href="https://www.instagram.com/abigail.kchairstylist?utm_source=ig_web_button_share_sheet&igsh=ZDNlZDc0MzIxNw==" target="_blank" class="externalLink">Follow Me On Instagram</a>
        <a href="https://maps.app.goo.gl/X1QNYv3NjdKM5Nto7" target="_blank" class="externalLink">Find Me On Google</a>

    </div>
</div>


<style lang="scss">
    @import '../../../static/style.scss'; 

    .Footer {
        background-color: #000;
        padding: 50px;

        .FooterContainer {
            text-align: center;


            a, p {
                color: #fff;
                margin: 15px auto;
            }

            a {
                cursor: pointer;
                text-decoration: underline;
            }
        }
    }

@media screen and (max-width: 820px) {
    .Footer {
        flex-direction: column-reverse;

        .FooterContainer {
            width: 100%;
        }
    }
}
</style>