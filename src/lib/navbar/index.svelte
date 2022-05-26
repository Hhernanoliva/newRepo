<script>
    const links = [
        {name: "Servicios", path: "servicios"},
        {name: "Contactos", path: "contactos"},
        {name: "Nosotros", path: "nosotros"},
        {name: "Ayuda", path: "ayuda"}
    ];
    
    const logoName = "new repo";
</script>

<nav>
    <div id="navbar" class="flex justify-between items-center px-2 py-3 max-h-20 ">

        <a id="logo" href="/" class="flex items-center">
            <img src="logopng2k.png" alt="" class="mx-2">
            <p class="text-3xl font-bold tracking-normal">{logoName}</p>
        </a>

        <div id="links" class="mr-2 hidden md:flex ">
            {#each links as link }
                <a href="{link.path}" class="px-4 text-base font-medium tracking-wide transition ease-in-out delay-100 hover:-translate-y-1 hover:scale-y-90  hover:bg-amber-200 duration-500 rounded-lg ...">{link.name}</a>
            {/each}
        </div>

        <div class="flex md:hidden">MENU</div>
    </div>
</nav>

<style lang="scss">
    @import url('https://fonts.googleapis.com/css2?family=Nunito:wght@700&display=swap');
    
    #logo{
        font-family: 'Nunito', sans-serif;
    }
    #navbar{
        background-color: rgba(255, 136, 0, 0.726);
        
    }
    #links{
        font-family: 'Montserrat', sans-serif;
        
    }


</style>