<script lang="ts">
  import MobileNav from "./MobileNav.svelte";

  let w: number,
    mobileNav: any,
    links: { title: string; link: string }[] = [
      {
        title: "Services",
        link: "Services",
      },
      {
        title: "Products",
        link: "Products",
      },
      {
        title: "Contact",
        link: "Contact",
      },
    ];

  let activeLink = {
    title: "Home",
    link: "/",
  };

  function scrollToTop() {
    document.body.scrollTo({ top: 0, behavior: "smooth" });
    document.documentElement.scrollTo({ top: 0, behavior: "smooth" });
  }

  function scrollTo(id: string) {
    const element = document.getElementById(id);

    if (element) {
      let newPosition = element.offsetTop - 70;
      document.body.scrollTo({ top: newPosition, behavior: "smooth" });
      document.documentElement.scrollTo({
        top: newPosition,
        behavior: "smooth",
      });
    }
  }
</script>

<svelte:window bind:innerWidth={w} />

<nav class="uk-navbar-container Nav">
  {#if w > 820}
    <div class="uk-container uk-flex uk-flex-between uk-flex-middle">
      <div class="uk-navbar uk-width-1-3">
        <div class="uk-navbar-left">
          <ul class="uk-navbar-nav">
            {#each links as link}
              <li>
                <button
                  on:click={() => {
                    scrollTo(link.link);
                    activeLink = link;
                  }}
                  class:isActive={link === activeLink}>{link.title}</button
                >
              </li>
            {/each}
          </ul>
        </div>
      </div>
      <button
        on:click={() => {
          scrollToTop();
        }}
        class="LogoWrap uk-width-1-3 uk-text-center">Hair by Abigail</button
      >
      <div class="BooKWrap uk-width-1-3 uk-flex uk-flex-right uk-flex-middle">
        <a
          class="Nav Nav-Book uk-button uk-button-default"
          href="https://abiferguson.glossgenius.com/services"
          >Book an Appointment</a
        >
      </div>
    </div>
  {:else}
    <div class="uk-container">
      <button
        class="uk-button uk-button-default uk-width-1-3 NavExpand"
        type="button"
        on:click={() => {
          mobileNav.showModal();
        }}><i class="fa-solid fa-bars"></i></button
      >
      <button
        on:click={() => {
          scrollToTop();
        }}
        class="LogoWrap uk-width-1-3 uk-text-center">Hair by Abigail</button
      >
      <div class="BooKWrap uk-width-1-3 uk-flex uk-flex-right uk-flex-middle uk-hidden">
        <a
          class="Nav Nav-Book uk-button uk-button-default"
          href="https://abiferguson.glossgenius.com/services">Book</a
        >
      </div>
    </div>
  {/if}
</nav>

<MobileNav bind:this={mobileNav} {links} bind:activeLink />

<style lang="scss">
  
  .Nav {
    background-color: #000;
    color: #fafdff;
    font-family: "Roboto", sans-serif;
    font-size: 17px;
    width: 100%;
    position: sticky;
    top: 0;

    .uk-container {
      box-shadow: 0px 0px 51px black;
      max-width: 100%;
      height: 70px;
    }

    button,
    a {
      color: #fafdff;
      text-transform: none;
      font-size: 17px;
      border: none;
      background: transparent;
      cursor: pointer;
    }

    .isActive {
      font-weight: bold;
    }

    .LogoWrap {
      font-size: 20px;
      cursor: pointer;
      font-family: "Satisfy", cursive;
    }

    .Nav-Book {
      font-size: 14px;
      border: none;
      width: fit-content;
      background: #fafdff;
      border-radius: 30px;
      color: #000;
    }
  }

  @media screen and (max-width: 820px) {
    .Nav {
      height: 50px;
      display: flex;
      align-items: center;
      flex-direction: row;

      .uk-container {
        background-color: unset;
        display: flex;
        align-items: center;
        flex-direction: row;
        height: 50px;
        margin: 0px;
        width: 100%;

        button {
          font-size: 20px;

        }
        
        .NavExpand {
          padding: 0px 0px 0px 20px;
          text-align: left;
        }
        .LogoWrap {
          width: unset;
        }

        .Nav-Book {
          height: unset;
        }
      }
    }
  }
</style>
