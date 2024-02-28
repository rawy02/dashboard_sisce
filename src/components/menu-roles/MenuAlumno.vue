<template>
    <v-navigation-drawer expand-on-hover rail class="bg-blue-grey-darken-3">
        <v-list>
            <v-list-item prepend-avatar="https://cdn-icons-png.flaticon.com/512/508/508970.png" class="text-center" title="SISCE"
                subtitle="ALUMNO"></v-list-item>
            <v-divider></v-divider>
            <v-list-item prepend-avatar="https://cdn-icons-png.freepik.com/512/194/194935.png"
                title="Rawy De Los Santos Fernandez" subtitle="202T0480">
                <!-- <v-btn>
                    Holoa
                </v-btn> -->
                

            </v-list-item>

        </v-list>

        <v-divider></v-divider>

        <v-list density="compact" nav>
            <v-list-item title="Opciones" value="opciones"></v-list-item>
            <v-list-item prepend-icon="mdi-folder" title="Datos Generales" value=""></v-list-item>
            <v-list-item prepend-icon="mdi-calendar" title="Horarios" value=""></v-list-item>
            <v-list-item prepend-icon="mdi-star" title="Calificaciones" value=""></v-list-item>
            <v-list-item prepend-icon="mdi-folder" title="Kardex" value=""></v-list-item>
            <v-list-item prepend-icon="mdi-account-multiple" title="Reinscripción" value=""></v-list-item>
            <v-list-item prepend-icon="mdi-star" title="Pagos" value=""></v-list-item>
        </v-list>

        
        <template v-slot:append>
          <div>
            <v-list-item prepend-icon="mdi-exit-to-app" class="bg-red-darken-4">
                Salir
            </v-list-item>
          </div>
        </template>

    </v-navigation-drawer>
</template>

<script>
export default {
    data: () => ({
        items: [
            { title: 'Click Me' },
            
        ],
    }),
}
</script>