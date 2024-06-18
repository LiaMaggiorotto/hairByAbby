<script lany="ts">
  import { goto } from "$app/navigation";

  let services = [
    {
      title: "Dimensional Color",
      desc: "Showcasing Balayage, Foilyage, Root Smudge, Color Melt, or any tailored multi-technique service. Infused with bond builders, gloss enhancements, and complemented by a personalized haircut, it's the artful fusion for captivating, multi-dimensional hair.",
      time: "3 to 4+ hours",
    },
    {
      title: '"Lived In" Blonding',
      desc: "A gentle lightening service curated for a seamless grow-out, employing multiple techniques. Enhanced with bond builders, gloss application, and paired with a tailored haircut, it's the ultimate blend for effortlessly radiant hair.",
      time: "3 to 4+ hours",
    },
    {
      title: "Root Touch Up",
      desc: "Offering precision and expertise, our root touch-up service seamlessly conceals pesky grey hairs at the root level, ensuring a natural, refreshed look for our clients' hair.",
      time: "1.5 hours",
    },
    {
      title: "Root to Ends",
      desc: "Provides complete strand coverage in a single hue. Paired with top-notch conditioners, bond builders, and a customized haircut, it's a holistic solution for vibrant, healthy-looking hair.",
      time: "3 hours",
    },
    {
      title: "Haircut",
      desc: "Specializing in medium to long hairstyles, I craft stunning bobs, lobs, and employ diverse layering techniques for a personalized look. Each session includes a rejuvenating shampoo, blow dry, and hot tool styling for a flawless finish.",
      time: "1 hour",
    },
    {
      title: "Gloss",
      desc: "Have a big event coming up, but you don't need a full color or appointment? Schedule a shine, color, or tone refresher between color services.",
      time: "1 hour",
    },
  ];
</script>

<div id="Services" class="Services uk-flex uk-flex-column uk-flex-middle">
  <h2>Services</h2>
  <div class="Services-wrap">
    <div class="uk-grid uk-grid-large uk-child-width-expand@s uk-text-center">
      {#each services as service}
        <div
          class="Services-service uk-flex uk-flex-column uk-flex-between uk-width-1-2"
        >
          <div>
            <h3>{service.title}</h3>
            <p>{service.desc}</p>
          </div>
          <small>{service.time}</small>
        </div>
      {/each}
    </div>
  </div>
  <button
    class="blackButton"
    on:click={() => {
      goto("https://abiferguson.glossgenius.com/services");
    }}>Book Appointment</button
  >
</div>

<style lang="scss">

  .Services {
    padding: 40px;
    color: #000;

    h2 {
      font-size: 75px;
      font-family: "Satisfy", cursive;
    }

    .Services-wrap {
      max-width: 80%;
      padding: 20px 5px;

      .Services-service {
        margin-bottom: 18px;
        text-align: left;

        p {
          margin: 20px 0px 10px;
        }
      }
    }
  }

  @media screen and (max-width: 820px) {
    .Services {
      h2 {
        font-size: 50px;
        margin: 0px;
      }

      .Services-wrap {
        max-width: 100%;
        padding: 20px 0px;

        .uk-grid {
          flex-direction: column;
          margin: 0px;
          padding: 0px;

          .Services-service {
            width: 100%;
            padding: 0px;

            h3 {
              font-size: 30px;
            }
          }
        }
      }
    }
  }
</style>
