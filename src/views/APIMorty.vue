<template>
    <div>

        <p>{{ memes }}</p>
        <div v-for="meme in memes" :key="meme.id">
            <ion-card>
                <img alt="Silhouette of mountains" :src="meme.image" />
                <ion-card-header>
                    <ion-card-title>{{meme.id}}</ion-card-title>
                    <ion-card-subtitle>{{ meme.name }}</ion-card-subtitle>
                </ion-card-header>

                <ion-card-content>
                </ion-card-content>
            </ion-card>
        </div>
    </div>
</template>
  
<script>
export default {
    data() {
        name: 'NewFecth'
        return {
            memes: [],
        };
    },
    mounted() {
        this.fetchMemes();
    },
    methods: {
        async fetchMemes() {
            try {
                const response = await fetch('https://rickandmortyapi.com/api/character');
                const data = await response.json();

                if (data.success) {
                    this.memes = data;
                } else {
                    console.error('Error al obtener memes');
                }

                console.log(data) 
            } catch (error) {
                console.error('Error en la solicitud:', error);
            }
        },
    },
};
</script>
  