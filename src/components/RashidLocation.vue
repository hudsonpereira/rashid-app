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
            const date = new Date();

            switch(date.getDay()) {
                case 1:
                    return 'Svargrond';
                case 2:
                    return 'Liberty Bay';
                case 3:
                    return 'Port Hope';
                case 4:
                    return 'Ankrahmun';
                case 5:
                    return 'Darashia'
                case 6:
                    return 'Edron'
                case 0:
                    return 'Carlin';
            }
        }
    }
}
</script>

