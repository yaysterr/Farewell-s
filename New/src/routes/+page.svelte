<script>
    let imageSrc1 = "doll-front.webp";
    let imageSrc2 = "jersey-front.png";
</script>

<style>
    img {
        transition: opacity 0.5s ease-in-out, transform 0.3s ease-in-out;
    }
    img:hover {
        transform: scale(1.05);
    }
</style>
<div class="flex flex-col items-center justify-center h-screen">
    <div class="">
        <a href="https://www.youtube.com/watch?v=xvFZjo5PgG0" >
            <img
                class="w-32 h-auto cursor-pointer"
                src={imageSrc1}
                alt=""
                on:mouseenter={() => (imageSrc1 = "doll-back.webp")}
                on:mouseleave={() => (imageSrc1 = "doll-front.webp")}
            />
        </a>
    </div>
    <div class="flex flex-col items-center justify-center ">
        <p>New Collection</p>
        <p>↓</p>
    </div>
</div>
<div class="flex flex-col items-center justify-center h-screen">
    <div class="">
            <img
                class="w-xl h-auto cursor-pointer" 
                src={imageSrc2}
                alt=""
                on:mouseenter={() => (imageSrc2 = "jersey-back.png")}
                on:mouseleave={() => (imageSrc2 = "jersey-front.png")}
            />
    </div>
        <p class="text-gray-400 mt-40">You want this for a Farewell's souvenir?</p>
        <button 
        class="cursor-pointer mt-5 px-6 py-2 bg-[#ddff00] text-black font-semibold rounded-full shadow-md hover:bg-[#99ff00] focus:outline-none focus:ring-2 focus:ring-blue-400 focus:ring-opacity-75 transition-transform transform hover:scale-105">
        Reserve
        </button>
</div>

