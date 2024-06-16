<script lany="ts">
</script>

<div id="Contact" class="Contact-wrapper uk-flex uk-flex-column uk-flex-middle">
  <h2>Get in touch.</h2>
  <div class="Contact uk-flex uk-flex-between">
    <div class="ContactContainer">
      <h4>Feel free to text me!</h4>
      <h5>
        <a
          href="sms://+14035550185?body=Hi!%20I%27m%20interested%20in%20scheduling%20an%20appointment.%20Please%20contact%20me."
          >(913) 213-8080</a
        >
      </h5>
    </div>
    <div class="ContactContainer">
      <h4>MOSS Studios</h4>
      <h5>3725 Broadway Blvd Suite 204</h5>
      <h5>Kansas City, MO 64111</h5>
    </div>
  </div>
  <img src="Abby_Contact.jpeg" alt="" />
</div>

<style lang="scss">
  @import "../../../static/style.scss";

  .Contact-wrapper {
    padding: 40px;
    color: #000;
    width: 80%;

    .Contact {
      padding: 20px 40px;
      width: 80%;

      .ContactContainer {
        a {
          font-size: 24px;
          text-align: center;
          font-family: "Quattrocento Sans", sans-serif;
          font-weight: bold;
          margin: 0px;
          color: #333;
          text-decoration: underline;
        }
      }
    }

    img {
      max-width: 60%;
      border-radius: 8px;
    }
  }

  @media screen and (max-width: 820px) {
    .Contact-wrapper {
      width: 100%;

      h2 {
        font-size: 50spx;
      }

      .Contact {
        width: 100%;
        flex-direction: column;
        gap: 40px;
        padding: 0px;
      }

      img {
        margin-top: 30px;
      }
    }
  }
</style>
