<script>
    import portfolio from "./Images/portfolioWebsite.webp";
    import frontEnd from "./Images/frontEnd.webp";
    import eersteWebsite from "./Images/eersteWebsite.webp";

    let portfolioItems = [
        {
            title: "Portfolio Website",
            imgUrl: portfolio,
            stack: ["Svelte", "Tailwind", "Nodejs"],
        },
        {
            title: "Frontend Keuzedeel",
            imgUrl: frontEnd,
            stack: ["Vue.js", "Tailwind", "Nuxt"],
        },
        {
            title: "Leerjaar 1 Eerste Website",
            imgUrl: eersteWebsite,
            stack: ["HTML", "CSS", "JS"],
        },
    ];
</script>

<div class="container mx-auto px-4 py-8 max-w-[65vw]">
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
        {#each portfolioItems as item}
            <div class="bg-white shadow-md rounded-lg overflow-hidden">
                <img
                    src={item.imgUrl}
                    alt={item.title}
                    class="w-full h-48 object-cover"
                />
                <div class="p-4">
                    <h3 class="text-xl font-semibold mb-2">{item.title}</h3>
                    <ul class="flex flex-wrap space-x-2">
                        {#each item.stack as tech}
                            <li
                                class="bg-gray-200 text-gray-800 px-3 py-1 rounded-full text-sm mb-2"
                            >
                                {tech}
                            </li>
                        {/each}
                    </ul>
                </div>
            </div>
        {/each}
    </div>
</div>
