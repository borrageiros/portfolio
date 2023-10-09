<script>
    import { page } from '$app/stores';
    let currentPath;
    $: currentPath = $page.url.pathname  ;
    let menuActive = $page.url.pathname == '/home' && true;

    function toggleMenu() {
        menuActive = !menuActive;
    }

    function preventDragStart(event) {
        event.preventDefault();
    }


</script>

<!-- Añadir el listener al elemento o al body si quieres que se aplique a todo -->
<svelte:body on:dragstart={preventDragStart} />
<nav id="menu" class:active={menuActive}>

    <!-- photo -->
    <!-- svelte-ignore a11y-img-redundant-alt -->
    <img id="personal_photo" src="/personal_photo.png" alt="Personal Photo">
    <span id="personal-photo-footer" >Adrián Borrageiros</span>
    
    <!-- ... menu ... -->
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <!-- svelte-ignore a11y-no-static-element-interactions -->
    <div id="menu-toggle" class="menu-icon" on:click={toggleMenu}>
        <div class="bar"></div>
        <div class="bar"></div>
        <div class="bar"></div>
    </div>
    <div class="menu-content">
        <ul class="menu-list">
            <li id="home" class:active-path={currentPath === '/'}>
                <a href="/" on:click={toggleMenu}><span>Home</span></a>
            </li>
            <li class:active-path={currentPath === '/about'}>
                <a href="/about" on:click={toggleMenu}><span>About</span></a>
            </li>
            <li class:active-path={currentPath === '/contact'}>
                <a href="/contact" on:click={toggleMenu}><span>Contact</span></a>
            </li>
        </ul>
    </div>
    

    <!-- ... social ... -->
    <div class="social-icons">
        <a href="https://github.com/borrageiros" target="_blank">
            <div class="icon github"></div>
        </a>
        <a href="https://www.linkedin.com/in/borrageiros/" target="_blank">
            <div class="icon linkedln"></div>
        </a>
        <a href="https://www.credly.com/users/adrian-borrageiros-mourelos/badges" target="_blank">
            <div class="icon credly"></div>
        </a>
    </div>
</nav>
