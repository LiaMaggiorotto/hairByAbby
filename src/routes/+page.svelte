<script lang="ts">
  import Header from "$lib/_components/Header.svelte";
  import Nav from "$lib/_components/Nav.svelte";
  import Products from "$lib/_components/Products.svelte";
  import Services from "$lib/_components/Services.svelte";
  import Footer from "$lib/_components/Footer.svelte";
  import Contact from "$lib/_components/Contact.svelte";
</script>

<div class="Wrapper uk-flex uk-flex-column uk-flex-middle">
  <Nav />
  <Header />
  <hr class="uk-width-3-4" />
  <Services />
  <hr class="uk-width-3-4" />
  <Products />
  <hr class="uk-width-3-4" />
  <Contact />
  <Footer />
</div>

<style lang="scss">

  .Wrapper {
    background-color: #fafdff;

    hr {
      border-top: 1px solid #000;
    }
  }
</style>

