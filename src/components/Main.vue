
<template>
    <v-container>
        <v-btn @click="knap">Tryk her</v-btn> 

      <v-layout row wrap justify-center align-center> 

        <!-- GRÆS -->
        <v-flex xs8 sm6 md4 lg3 v-for="pokemon in pokemonData" :key="pokemon.id">
             <div v-if="pokemon.types[0].type.name == 'grass'">
                <v-card class="ma-3" max-width="300" height=400px color="#86f88e"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-grass</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
             </div>

           

             <!-- VAND -->
            <div v-if="pokemon.types[0].type.name == 'water'">
                <v-card class="ma-3" max-width="300" height=400px color="#72a9e1"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-water</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
             </div>
        
            <!-- FIRE -->
            <div v-if="pokemon.types[0].type.name == 'fire'">
                <v-card class="ma-3" max-width="300" height=400px color="#f88e86"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-fire</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
             </div>


            <!-- INSEKT -->
            <div v-if="pokemon.types[0].type.name == 'bug'">
                <v-card class="ma-3" max-width="300" height=400px color="#cfd875"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-bug</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
             </div>


            <!-- NORMAL -->
            <div v-if="pokemon.types[0].type.name == 'normal'">
                <v-card class="ma-3" max-width="300" height=400px color="#fff2cc"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-circle-double</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>


            <!-- Electric -->
            <div v-if="pokemon.types[0].type.name == 'electric'">
                <v-card class="ma-3" max-width="300" height=400px color="#ffff7f"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-lightning-bolt</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>

        
            <!-- Electric -->
            <div v-if="pokemon.types[0].type.name == 'ground'">
                <v-card class="ma-3" max-width="300" height=400px color="#dfd8c1"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-liquid-spot</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>


            <!-- Psycic -->
            <div v-if="pokemon.types[0].type.name == 'poison'">
                <v-card class="ma-3" max-width="300" height=400px color="#b266b2"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-skull</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>


            <!-- Psycic -->
            <div v-if="pokemon.types[0].type.name == 'psychic'">
                <v-card class="ma-3" max-width="300" height=400px color="#ffd9df"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-eye</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>

            <!-- Fairy -->
            <div v-if="pokemon.types[0].type.name == 'fairy'">
                <v-card class="ma-3" max-width="300" height=400px color="#f7b1ea"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-star-four-points</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>


            <!-- Fighting -->
            <div v-if="pokemon.types[0].type.name == 'fighting'">
                <v-card class="ma-3" max-width="300" height=400px color="#db8c8c"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-mixed-martial-arts</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>


            <!-- rock -->
            <div v-if="pokemon.types[0].type.name == 'rock'">
                <v-card class="ma-3" max-width="300" height=400px color="#e1b166"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-image-filter-hdr</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>

            <!-- ghost -->
            <div v-if="pokemon.types[0].type.name == 'ghost'">
                <v-card class="ma-3" max-width="300" height=400px color="#71609e"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-ghost</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>


            <!-- steel -->
            <div v-if="pokemon.types[0].type.name == 'steel'">
                <v-card class="ma-3" max-width="300" height=400px color="#a084e7"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-bolt</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>



            <!-- ice -->
            <div v-if="pokemon.types[0].type.name == 'ice'">
                <v-card class="ma-3" max-width="300" height=400px color="#92CBFF"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-snowflake</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>


            <!-- flying -->
            <div v-if="pokemon.types[0].type.name == 'flying'">
                <v-card class="ma-3" max-width="300" height=400px> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-bird</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>


            <!-- dragon -->
            <div v-if="pokemon.types[0].type.name == 'dragon'">
                <v-card class="ma-3" max-width="300" height=400px color="#2986CC"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-snake</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>


            <!-- dark -->
            <div v-if="pokemon.types[0].type.name == 'dark'">
                <v-card class="ma-3" max-width="300" height=400px color="#666666"> 
                    <v-layout>
                    <v-img width="100px" :src="imgurls[pokemon.id]">
                        <v-app-bar flat color="rgba(0,0,0,0)">
                            <v-toolbar-title class="text-h6 pl-0">
                                <v-card-title><v-icon left>mdi-moon-waxing-crescent</v-icon>{{ pokemon.name }}</v-card-title>
                            </v-toolbar-title> 
                            <v-spacer></v-spacer> 
                            #{{ids[pokemon.id]}}
                        </v-app-bar>
                    </v-img>
                    </v-layout>
                </v-card>
            </div>

        </v-flex>
        <!-- {{pokemonCards}} -->

        <!-- <v-flex xs12 sm6 md4 lg3 v-for="pokemon in pokemonCards">
            <v-card class="ma-3" max-width="400" height=400px>
                {{pokemon.text}}
            </v-card>
        </v-flex> -->

      </v-layout>
  </v-container>
</template>

<script>
    var Pokedex = require('pokedex-promise-v2');
    var P = new Pokedex();

  export default {
    name: 'Main',

    // Test data ideelt set bliver det hentet fra pokemon api
    data: () => ({
        NoOfPokemon: 0,
        pokemonNames: [],
        imgurls: [],
        types: [],
        ids: [],
        pokemonData: [],
    
        cards: [{}
        ],
    }),
    methods: {
        knap(){
            console.log("du trykkede, du fik:")
            console.log("Antal pokemon (i alt): ", this.NoOfPokemon)
            console.log("Antal pokemon (vi har kigget på):", this.ids.length)
            console.log(this.pokemonData[100])
            // console.log(this.imgurls)
        

            
        },

    },
    created() {
        console.log(P)

        const printListe = async () =>{
            const l = await P.getPokemonsList()
            this.NoOfPokemon = l.count          
            for (let i = 0; i <= 898; i++){
                var id = ''
                if (i < 10){
                    id = '00' + (i)
                } else if (i < 100) {
                    id = '0' + (i)
                } else if (i < 1000) {
                    id = i 
                }
                this.ids.push(id)
                this.pokemonNames.push(l.results[i].name)

                await fetch(l.results[i].url)
                    .then((response) => response.json())
                    .then(data => {
                        this.pokemonData.push(data)
                        this.imgurls.push(`https://assets.pokemon.com/assets/cms2/img/pokedex/full/${id}.png`)
                    })
                    .catch( )
                
            }

        }
        console.log(printListe())
    }
  }
</script>


<style scoped>
    .v-text-field--outlined >>> fieldset {
    border-color: rgba(192, 0, 250, 0.986);
    }
</style>

<style>
    .grass{
        color: "#86f88e";
    }
</style>