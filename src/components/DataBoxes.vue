<template>
<div class="grid md:grid-cols-2 gap-4" >
    <!--Box 1-->
    <div class="shadow-md bg-blue-100 p-10 text-center rounded">
        <h3 class="text-3x1 text-blue-900 font-bold mb-4">Cases</h3>
        <div class="text-2x1 mb-4">
            <span class="font-bold">New:</span>
            {{ stats.NewConfirmed }}
        </div>
        <div class="text-2x1 mb-4">
            <span class="font-bold">Total:</span>
            {{ stats.TotalConfirmed }}
        </div>
    </div>
    <!--Box 2-->
    <div class="shadow-md bg-blue-200 p-10 text-center rounded">
        <h3 class="text-3x1 text-blue-900 font-bold mb-4">Cases</h3>
        <div class="text-2x1 mb-4">
            <span class="font-bold">New:</span>
            {{ stats.NewDeaths }}
        </div>
        <div class="text-2x1 mb-4">
            <span class="font-bold">Total:</span>
            {{ stats.TotalDeaths }}
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'DataBoxes',
    props: ['stats']
}

</script>