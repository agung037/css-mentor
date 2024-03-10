<script>
    import image from '$lib/images/illustration-article.svg';
    import avatar from '$lib/images/image-avatar.webp'

    let isHovered = false;

    function handleMouseEnter(){
        isHovered = true

    }

    function handleMouseLeave(){
        isHovered = false
    }

    function clickHandler(){
        alert("you clicked me!")
    }
</script>

<style>
    .main {
        font-family: 'Figtree', sans-serif;
        background-color: hsl(47, 88%, 63%);
        display: flex;
        align-items: center;
        justify-content: center;
        height: 100vh;
    }


</style>

<div class="main h-screen">
  
    <!-- box -->
    <div class="border border-gray-800 w-80 bg-white rounded-xl flex flex-col p-4 text-white transition-transform transform {isHovered ? 'hover:shadow-[15px_15px_0px_0px_rgba(0,0,0)]' : 'shadow-[5px_5px_0px_0px_rgba(0,0,0)]'}">
        <img class="w-full h-50 object-cover rounded-xl mb-5" src="{image}" alt="Card Image">
        
        <div class="font-bold bg-yellow-400 text-black rounded-md w-1/3 text-center">
            <p>Learning</p>
        </div>

        <div class="my-3 text-base text-black">
            <p>Published 21 Dec 2023</p>
        </div>

        <div class="my-3 text-base text-black">
            <a href="#" on:click={clickHandler} on:mouseenter={handleMouseEnter} on:mouseleave={handleMouseLeave} class="text-2xl font-extrabold {isHovered ? 'text-yellow-400 cursor-pointer' : 'text-black'}">HTML & CSS foundation</a>
        </div>

        <div class="my-3 text-base text-gray-500">
            These languages are the backbone of every website, defining structure, content, and presentation.
        </div>

        <div class="flex items-center mt-3">
            <span>
                <img class="size-10" src="{avatar}" alt="person avatar">
            </span>
            <span class="mx-4">
                <p class="text-black font-black">Greg Hopper</p>
            </span>
        </div>
    </div>
    <!-- end box -->

</div>

