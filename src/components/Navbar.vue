<template>
    <nav>
        <v-toolbar v-app>
            <!-- @click="drawer = !drawer" -->
            <v-app-bar-nav-icon variant="text" color="blue-grey-lighten-1" @click="rail = false"
                style="margin-left: 60px;"></v-app-bar-nav-icon>
            <!-- Titulo TODORAWY -->
            <v-toolbar-tittle class="text-h6 text-blue-grey-lighten-1">
                <span class="font-weight-thin">TODO</span>
                <span class="font-weight-medium">RAWY</span>
            </v-toolbar-tittle>
            <v-spacer></v-spacer>
            <!-- Boton SIGN OUT -->
            <v-btn variant="flat" color="grey-lighten-2">
                <span class="text-blue-grey-lighten-1">Sign Out</span>
                <v-icon icon="mdi-exit-to-app" color="blue-grey-lighten-1"></v-icon>
            </v-btn>
        </v-toolbar>
        <!-- Menu a la izquierda -->
        <!-- <MenuAlumno /> -->
        <v-navigation-drawer v-model="drawer" :rail="rail" permanent @click="rail = false" expand-on-hover
            class="bg-blue-grey-darken-3">
            <v-list-item prepend-avatar="https://cdn-icons-png.flaticon.com/512/508/508970.png" title="SISCE">
                <template v-slot:append>
                    <v-btn variant="text" icon="mdi-chevron-left" @click.stop="rail = !rail"></v-btn>
                </template>
            </v-list-item>

            <v-divider></v-divider>

            <v-list-item prepend-avatar="https://cdn-icons-png.freepik.com/512/194/194935.png"
                title="Rawy De Los Santos Fernandez">
                <!-- <template v-slot:append>
                    <v-btn variant="text" icon="mdi-chevron-left" @click.stop="rail = !rail"></v-btn>
                </template> -->
            </v-list-item>



            <v-divider></v-divider>

            <v-list density="compact" nav>
                <v-list-item prepend-icon="mdi-home-city" title="Home" value="home"></v-list-item>
                <v-list-item prepend-icon="mdi-account" title="My Account" value="account"></v-list-item>
                <v-list-item prepend-icon="mdi-account-group-outline" title="Users" value="users"></v-list-item>
            </v-list>
            <template v-slot:append>
                <div>
                    <v-list-item prepend-icon="mdi-exit-to-app" class="bg-red-darken-4">
                        Salir
                    </v-list-item>
                </div>
            </template>
        </v-navigation-drawer>
    </nav>
</template>

<script>
// import MenuAlumno from '@/components/menu-roles/MenuAlumno'
export default {
    // components: { MenuAlumno },
    data() {
        return {
            drawer: true,
            rail: true,
        }
    },
}
</script>