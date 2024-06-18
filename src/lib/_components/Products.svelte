<script lany="ts">
</script>

<div
  id="Products"
  class="Products-wrapper uk-flex uk-flex-column uk-flex-middle"
>
  <h2>Products</h2>
  <div class="Products uk-flex uk-flex-around">
    <div class="Products-section uk-flex uk-flex-column uk-flex-middle">
      <h3>Personalized Hair Care</h3>
      <div
        class="imageContainer"
        style="background: url(Goldie_Locks_Shampoo.jpeg); background-position: center;
    background-repeat: no-repeat; background-size: contain; border-radius: 8px;"
      ></div>
      <p class="uk-text-center">
        Get your personalized hair care routine through Goldie Locks, a company
        focused on enhancing the experience you can have with your hair from the
        inside out.
      </p>
      <a
        target="_blank"
        class="blackButton"
        href="https://goldielocks.com/?sca_ref=2599066.5T9VJPRpfc&utm_medium=uppromote&utm_source=affiliates"
        >Shop Now</a
      >
    </div>
    <div class="Products-section uk-flex uk-flex-column uk-flex-middle">
      <h3>Invisible Bead Extensions®</h3>
      <div
        class="imageContainer"
        style="background: url(Balayage_Blonde.jpeg); background-position: center; background-repeat: no-repeat; background-size: cover;  border-radius: 8px;"
      ></div>
      <p class="uk-text-center">
        I am certified in Invisible Bead Extensions® (IBE®), the #1 most
        requested hand-tied extension method. Let’s chat about if this
        damage-free extension option is right for you.
      </p>
      <a
        target="_blank"
        class="blackButton"
        href="https://www.invisiblebeadextensions.com/blog/all-about-ibe"
        >Learn More</a
      >
    </div>
  </div>
</div>

<style lang="scss">
  .Products-wrapper {
    padding: 40px;
    .Products {
      padding: 40px;
      color: #000;
      width: 90%;

      .Products-section {
        width: 569px;

        .imageContainer {
          width: 395px;
          height: 445px;
        }

        p {
          width: 450px;
          max-width: 100%;
        }

        a {
          text-decoration: none;
        }

        a:hover {
          color: #fafdff;
        }
      }
    }
  }

  @media screen and (max-width: 1023px) {
    .Products-wrapper {
      padding: 40px;

      h2 {
        font-size: 50px;
      }

      .Products {
        padding: 0px;
        width: 100%;
        flex-direction: column;
        gap: 50px;

        .Products-section {
          width: 100%;
          margin: 0px;

          h3 {
            font-size: 30px;
          }

          .imageContainer {
            height: 353px;
            width: 315px;
          }

          p {
            width: 100%;
          }
        }
      }
    }
  }
</style>
