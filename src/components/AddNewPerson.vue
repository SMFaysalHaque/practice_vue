<template>
    <div>
        <div class="flex justify-between items-center border border-stone-200 border-b-0 w-4/12 px-5 py-2 mt-5 mx-auto">
            <p>Add New Person</p>
            <button @click="$emit('close')" class="border border-red-600 hover:bg-red-500 rounded-md px-5 py-2">Close</button>
        </div>
        <div class="border border-stone-200 w-4/12 px-5 py-5 mx-auto ps-16 space-y-2">
            <p>Name: <input class="border rounded-lg contrast-more:border-slate-400 focus:outline-none focus:border-sky-500 focus:ring-1 focus:ring-sky-500 ms-1" type="text"></p>
            <p>Mobile: <input class="border rounded-lg contrast-more:border-slate-400 focus:outline-none focus:border-sky-500 focus:ring-1 focus:ring-sky-500 ms-1" type="text"></p>
            <button class="border border-sky-600 hover:bg-sky-500 rounded-md px-6 py-1">Save</button>
        </div>
        <div>

        </div>
    </div>
</template>

<script>
    export default {
        name: 'AddNewPerson',
        props: {
            informations: {
                type: Array,
            },
        },
        emits: ['close'],
        components: {
        },
        data() {
            return {
                
            }
        },
        methods: {
            
        },
    }
</script>

<style lang="scss" scoped>

</style>