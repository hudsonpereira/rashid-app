<template>
    <div>
        <img src="../assets/rashid-npc.gif" alt="Rashid">

        <p class="my-3">Rashid is at {{ location }}</p>
    </div>
</template>

<script>
export default {
    computed: {
        location: () => {
            const location = 'Svargrond';

            return location;
        }
    }
}
</script>

