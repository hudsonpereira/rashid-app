<template>
    <div>
        <input class="form-control" type="text" placeholder="Enter the highest level" v-model="level">

        <p class="my-3 text-justify" v-if="minPartyLevel">{{ minPartyLevel }}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            level: null,
            minPartyLevel: null,
        }
    },
    watch: {
        level: function(val) {
            const level = parseInt(val);

            if (Number.isInteger(level)) {
                this.minPartyLevel = 'Min level is: ' + Math.round(val / 3 * 2)
            } else {
                this.minPartyLevel = null;
            }
        }
    }
}
</script>

