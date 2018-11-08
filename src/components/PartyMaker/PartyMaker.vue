<template>
    <div>
        <div class="form-row">
            <div class="col col-md-10">
                <input type="text" class="form-control" placeholder="Type your name here." v-model="characterName">
            </div>
            <div class="col">
                <button class="btn btn-primary" v-on:click="findPartyHandler">Find party</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            characterName: null
        }
    },
    methods: {
        findPartyHandler: () => {
            const url = "https://api.tibiadata.com/v2/characters/" + encodeURIComponent(this.characterName) + ".json"

            fetch(url, {
                mode: 'cors',
                credentials: "same-origin"
            }).then(function() {
                alert('done')
            });
        }
    }
}
</script>

