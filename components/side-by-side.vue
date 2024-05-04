<template>
    <div class="bg-white">
        <h2 class="text-3xl font-bold leading-10 tracking-tight text-gray-900">FAQS</h2>
        <div class="mx-auto max-w-7xl divide-y divide-gray-900/10 px-6 py-24 sm:py-32 lg:px-8 lg:py-16">
            <h2 class="text-2xl font-bold leading-10 tracking-tight text-gray-900">Who's who?</h2>
            <dl class="mt-10 space-y-8 divide-y divide-gray-900/10">
                <div v-for="faq in faqs" :key="faq.id" class="pt-8 lg:grid lg:grid-cols-12 lg:gap-8">
                    <dt class="text-base font-semibold leading-7 text-gray-900 lg:col-span-5">{{ faq.question }}</dt>
                    <dd class="mt-4 lg:col-span-7 lg:mt-0">
                        <p class="text-base leading-7 text-gray-600">{{ faq.answer }}</p>
                    </dd>
                </div>
            </dl>
        </div>
    </div>
</template>
  
<script setup>
const faqs = [
    {
        id: 1,
        question: "Best looking",
        answer:
            "Based sa google forms, si Jepe aka John Paul Delos Santos",
    },
    {
        id: 2,
        question: "GF/BF Material",
        answer:
            "Based sa google forms, tied si charls og erek",
    },
    {
        id: 3,
        question: "Green flag",
        answer:
            "Based sa google forms, tied si haryen og bals??? questionable si bals but ok?",
    },
    {
        id: 4,
        question: "Red flag",
        answer:
            "Based sa google forms, the one and only Jonhyl Balsamo",
    },
    {
        id: 5,
        question: "Biggest Simp",
        answer:
            "Based sa google forms, si Robert Jims Aquino. Move on move on sad doy",
    },
]
</script>