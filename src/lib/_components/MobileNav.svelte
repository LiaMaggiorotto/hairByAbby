<script lang="ts">
    export let links: { title: string; link: string }[];
    export let activeLink: { title: string; link: string };

</script>

<div class="uk-offcanvas">
  <div class="uk-offcanvas-bar">
    <button class="uk-offcanvas-close" type="button"></button>

    <ul class="uk-navbar-nav">
        {#each links as link}
          <li>
            <button
              on:click={() => {
                scrollTo(link.link);
              }}
              class:isActive={link === activeLink}>{link.title}</button
            >
          </li>
        {/each}
      </ul>
  </div>
</div>
