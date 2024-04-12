<script>    
  import logo from '/logo.png';
  import { base } from "$app/paths";
</script>
<svelte:head>
    <link rel="stylesheet" href="{base}/pagelayout.css">
</svelte:head>
<header class="header clearfix">
    <a href="/" title="SAV DDTH">
        <img src={logo} alt="Logo" class="header__logo" />
    </a>
    <form action="/content/search" method="get" id="header-search-form">
        <input type="text" value="" id="search" name="SearchText">
        <input name="SearchButton" class="submit" type="submit" value="Rechercher">
    </form>
    <!-- Add other header content here -->
  </header>
<div id="page" class="container">
    <slot></slot>
</div>
<footer class="footer">
    <a href="/">Contactez-nous</a>
</footer>
