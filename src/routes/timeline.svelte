<script>
    let timeline = [
        {
            year: "today",
            title: "Frontend Keuzedeel",
            duration: "4 maanden",
            details:
                "Op school hebben we kennis gemaakt met Vuejs en Bootstrap.css. Samen met GitHub voor versie beheer hebben we een basis gekregen voor webdevelopment. Ik heb een site gemaakt voor een dieren asiel. Natuurlijk is die responsive en makelijk veranderingen in te brengen. binnenkort hebben we hier examen voor maar die zal makelijk te doen moeten zijn",
        },
        {
            year: "2023",
            title: "Stage Innosportlab",
            duration: "4 maanden",
            details:
                "Mijn eerste stage! Ik heb hier gebruik gemaakt van PHP, CSS, SQL en PHPMyAdmin. Ik heb aan een website en database gewerkt. Met deze database kunnen we alle resultaten van turn sport wedstrijden opslaan. En ze weer laten zien op de website. Maar waarom? we hadden het probleem dat niet elke score pdf het zelfde formaat volgde. Dus dat hebben we met veel stoei en puzzellen op gelost!",
        },
        {
            year: "2022",
            title: "Koning Willem 1 College",
            duration: "4 Jaar",
            details:
                "Op het College hebben we van alles gehad! we begonnen met HTML, CSS en Js. Met die 3 hebben we statische en responsive website gemaakt. daarna hebben we daar PHP aan toegevoegt. En met PHP kwam ook SQL zodat we databases konden gebruiken in onze websites. In de 3rde hebben we c#. Hier gebruikte we vooral windows forms samen met SQL om naja... windows forms te maken. Daarna hebben we XAML gedaan met SQLite om apps te maken voor IOS en Android. En nu hebben we Python op de raspberry Pi. We maken een puzzle room met hulp van die 2. ",
        },
        {
            year: "2022",
            title: "Zelfstandige Chef Opleiding",
            duration: "6 maanden",
            details:
                "Dit is weer een hele anderen kant dan ICT. Koken vond ik altijd erg leuk en ik wist nog niet zeker wat ik wouw doen, dus ik had gekozen voor de kok opleiding. Uiteindelijk ben ik er achter gekomen dat koken leuk is... maar niet voor klanten 8 uur op een dag. Daarna heb ik besloten om naar de Software Opleiding te gaan van het KW1C",
        },
    ];
</script>

<div class="container mx-auto px-4 py-8 max-w-3xl">
    <div class="relative border-l-4 border-gray-200">
        {#each timeline as event}
            <div class="mb-8 ml-6">
                <div
                    class="absolute w-6 h-6 -left-3 bg-teal-500 rounded-full border-2 border-white"
                ></div>
                <p class="text-sm text-gray-500">{event.year}</p>
                <h2 class="text-xl font-semibold">{event.title}</h2>
                <p class="text-gray-600">{event.duration}</p>
                <p class="mt-2 text-gray-700">{event.details}</p>
            </div>
        {/each}
    </div>
</div>
