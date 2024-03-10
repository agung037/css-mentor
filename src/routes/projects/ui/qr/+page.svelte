
<script>
    import image from '$lib/images/image-qr-code.png';
</script>

<div class="main h-screen bg-slate-200 flex items-center justify-center">

    <!-- my card -->
    <div class="p-3 m-5 max-w-md bg-white rounded-lg overflow-hidden shadow-md w-full md:w-2/3 lg:w-1/2 xl:w-1/3">
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img class="w-full h-50 object-cover rounded-lg" src="{image}" alt="Card Image">
        <div class="p-4">
            <div>
                <h2 class="text-3xl font-semibold mb-2 text-center">improve your front-end skill by building projects</h2>
            </div>
            <div>
                <p class="text-xl text-gray-400 text-center">Scan the QR code to visit Frontend Mentor and take your coding skills to the next level</p>
            </div>
        </div>
    </div>
    <!-- end of my card -->
</div>

<style>
    @tailwind base;
    @tailwind components;
    @tailwind utilities;

    /* apply garamond font on all of page */
    body {
        font-family: 'Roboto';
    }

</style>
