<script lang="ts">
</script>

<div id="Header" class="Header uk-flex">
  <div class="Header-image uk-width-1-2 uk-flex uk-flex-center">
    <img src="Abby_Header.jpeg" alt="" />
  </div>
  <div class="Header-text uk-flex uk-flex-center uk-flex-column uk-width-1-2">
    <h1>Hair By Abigail</h1>
    <p>
      I’ve been a hairstylist in both Downtown and Midtown Kansas City since I
      was twenty years old. For so many years I believed the beauty industry was
      something I just “fell” into. Now 20 years later, I tell a different
      story. Having been invited to leave twice for what seemed like incredible
      opportunities, I continuously found myself quickly crawling back to this
      industry with so much love and gratitude.

      <br />
      <br />
      Hair color is what does it for me! I get goosebumps when I see how even just
      a slight shift in a color formulation or placement changes everything for my
      client!
      <br />
      <br />

      As a blonde/bronde color specialists, I understand the importance of
      continuous investment in hair education. I strive to ensure that my
      techniques and products are of the highest quality available.
      <br />
      <br />

      My goal is to make my clients feel beautiful from the outside in. Because
      when you look good, you feel good, and when you feel good, you do good!
    </p>
  </div>
</div>

<style lang="scss">
  @import "../../../static/style.scss";
  //#000;
  // #fafdff;

  .Header {
    padding: 40px;
    color: #000;
    gap: 40px;

    .Header-image {
      img {
        max-width: 35vw !important;
        border-radius: 4px;
      }
    }

    .Header-text {
      margin-right: 45px;
    }
  }

  @media screen and (max-width: 1024px) {
    .Header {
      .Header-image {
        img {
          max-width: 45vw !important;
        }
      }
    }
  }

  @media screen and (max-width: 820px) {
    .Header {
      flex-direction: column;

      .Header-image,
      .Header-text {
        width: 100%;
      }

      .Header-image {
        img {
          width: 100% !important;
          max-width: 100% !important;
        }
      }

      .Header-text {
        margin: 0px;

        h1 {
          font-size: 50px;
          margin: 0px;
        }
      }
    }
  }
</style>
