<template>
        <v-footer
        app
        padless
        absolute
        >
                <v-card class="footer"
                width="100%"
                color="#42b883"
                >
                        <v-card-title>
                        <div>Haschul&copy; 2020 - {{ new Date().getFullYear() }}</div>

                        </v-card-title>
                                                <v-spacer></v-spacer>
                        <v-card-title>
                        <div>Retrouvez nous sur</div>
              <div class="flex">
                <a class="icons" href="https://www.linkedin.com/in/william-azis-09601127/"><v-icon >mdi-linkedin</v-icon> </a>
                <v-icon >mdi-facebook</v-icon>
                <v-icon >mdi-twitter</v-icon>
                <v-icon >mdi-instagram</v-icon>
              </div>
                        </v-card-title>
                </v-card>

        </v-footer>
</template>

<style scoped>
        .footer {
                display:flex;
                white-space: nowrap;
                }
        div {
                padding-left: 10x;
                padding-right: 10px;
                color:"red";
                font-size: 16px;
            }
.icons {
  margin-right: 1%;
  margin-left: 1%;
  text-decoration: none;
}
</style>