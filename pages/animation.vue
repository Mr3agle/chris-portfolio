<template>
  <div>
    <v-row class="ml-1 mt-5">
      <div class="display-2">Sketches y Diseño de Personajes</div>
      <p
        class="mt-3"
      >Estos sketches fueron creados con l intención de dar vida a diferentes personajes, además de verlos en diferentes situaciones. Es el primer paso en el proceso de animación.</p>
    </v-row>
    <v-carousel class="my-5" hide-delimiters>
      <v-carousel-item v-for="(item,i) in sketches" :key="i" :src="item.src"></v-carousel-item>
    </v-carousel>

    <v-divider class="my-12" />

    <v-row class="ml-1 mt-5">
      <div class="display-2">Pruebas de Lápiz</div>
      <p
        class="mt-3"
      >Estas son animaciones simples para probar varios conceptos o movimientos antes de integrarlos a una animación final. Es el segundo paso en el proceso de animación.</p>
    </v-row>
    <v-carousel class="my-5" hide-delimiters>
      <v-carousel-item v-for="(item,i) in handraws" :key="i">
        <v-row justify="center">
          <video :src="item.src" controls></video>
        </v-row>
      </v-carousel-item>
    </v-carousel>

    <v-divider class="my-12" />

    <v-row class="ml-1 mt-5">
      <div class="display-2">Animación a Blanco y Negro</div>
      <p
        class="mt-3"
      >Animaciones casi finales, donde se asegura que las animaciones y concepto funcionen bien en conjunto antes de darles color. Es el tercer paso en el proceso de animación.</p>
    </v-row>
    <v-carousel class="my-5" hide-delimiters>
      <v-carousel-item v-for="(item,i) in bw" :key="i">
        <v-row justify="center">
          <video :src="item.src" controls height="500px"></video>
        </v-row>
      </v-carousel-item>
    </v-carousel>

    <v-divider class="my-12" />

    <v-row class="ml-1 mt-5">
      <div class="display-2">Producto Final</div>
      <p
        class="mt-3"
      >Animación llamada CHEESE que cuenta una historia de acerca de la discriminación, aquí vemos todos los procesos de animación trabajar en conjunto.</p>
    </v-row>
    <v-row justify="center">
      <video class="mt-5" src="/video/cheeseMockUp.mp4" controls height="500px"></video>
    </v-row>
  </div>
</template>


<script>
export default {
  data() {
    return {
      sketches: [
        {
          src: 'https://lh3.googleusercontent.com/tcmJNOTOLc8QKDzX-aiiThhsdXUHug3DGrsWbXChjTJnwHhb8_wHGVvHJ8viES7uSk6H_irwNjcHA58cCHOcMTxBIyRu5iOZ_FB_Az4px2ZobRDHOJbQXMHosRa_cI3SDmYCYx9V433fA24AJyrHBVvPyoTliFzznyJFudVZd-3VYBVC32XygRMESR11uYc4QM8UgrAnXkJZL7EOQZcuCqj7U5IxbShZ4cvcPaBC9akh4YKrtMF48eYEL4FUfcZlTDtC6dXeOKVCJDZQNbCUd6ciGSD-HE7wdI4DP5oyeyJQuHQzxUtsbOj70pFSm8SOL35Ji5UcLH-O7ukDrt_QRwPL0hXq5F0DdzMQkCT7uD9YxFb2suIavd7nshf9CmNijEfGsJ_Zy32uaL39eU5MWcGZB4X393Ea3FPXPpcC2RGPE6mTitYKwFzwQUy4D_or32a3U8Udwn0zK7XLHAU0uh7LT79VYIlXX8lab4288e83BxKTC55al3KQ8ez6RZPzicrHyKuQcuCG3bv9B6OOJH5VU4BZGa7kOuoOVHBxqwNXUPIsqqr5nRRlECJVTcYMR86jB81twFQVWzn5zJ6Go1RO5RwX-8zJqYb6zqqgWgLCIlkI9qGU0a-96vAX1I8_T_2YGOMD1iSHEW7iTSDV4BL39I2kIAtmtEN9HYK5U2ZiU5ASlcF0ACvSJkMcSx0an0QoFnm1yftAONMleppdM-KS3MDCLqubVdX9ciMcf8C7TGyq8s6LiYA=w1278-h852-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/nicYETc-xs1yLvGia-y_q3o_NdzN5bmnq4KH8-c14Dhtp69iPDWTGsQ_LKZYiizo8gwEnrVzY5dHhScSJ8ZTOH2xbjPn03GQKMus4Nqv14eAoupQn8Z0_27O_t6znUldSBWk_29oH39BL0UOtXNE7o9fmqX6XQw44lLCrdqsxIvAtQhf8ocFSzlkKfUs5kXnHej_o3Id1AM2DmKPBEFqvmSW_B_TZyoZ7JQj4AO8aPbmdvng_VhxV5apFIW2CIDOdRbANKLP0b5mF9cGBbZyUH3gFumy6dwJ0tnQ-kka7ebEUVwr1r7pipHHtqJvJihz8rIU2JIeE393st2cTm5XntVCC6tmmq3PO9IsQHfOvKuL6663ABHyUDbXxISFu0b-Z4LIjc3SwdEya-5wieR9kH7-hr0WPaRDZycqP54Pfzjd8Be8NdV5x5kclfMpI2wP8jiTxsYCtEwtal6rlJCAeh1N1hL70OAd0c2urXevu2MwJ65ovhE7JYq7LYygbZaFkpaKesIp4q86VO_uu6sISefhRTyQOnkXWGhBBGsnrfevSpU6w5FpfFKZb0DRsmGyotLuooGz6RQN02cnjWa1oLExw2DaLwchgwVkO29C8Bj-x6fc27DGZJbwXe1NOaHSgvKTGFVLuxdvkZc-XHWLxB0zUroCEPYaNYE3QF4BGz_lHQwVus8S4X9vqsmKmImIgQ1J_DHoiqYTW-fVULnz525aELxArNVS5qw0ky6eOcylqW9EcHzG9Zo=w1278-h852-no',
        },
        {
          src: 'https://lh3.googleusercontent.com/cIQSv8YNEf1ceNOPhq5Et9ntRoVY6mnafnnH9LavOe9JUnv-_vTMJk2m2LNivpBICeGFmB0uQlOHadOMnQWp9Gk9x9xhDjWUTrOOUsS8M8mfCeeTQth6cFYA_felD8YLpRbo8gM780bVciUSZVfhgDmrNKCMgg8RTjIrrQEKUGzsNw03z-Vvp9OeVY3945SUPjy8N7HMcxZWZZyeq1RZyiUhe1a4H-aQfYEbDPRIyRd4bFh8Hn6CMNLIkRBtcqfZRXki8sXaYi5XHXUlJqGYXAvAeQD66Y1sTpenMXlJ9kS29_OrIxxVPvjpSQ_Dm9yHi4ehht4VyXbE7LreRmO3wsKJ7O48uxX6Pivs5SyZTkTyJS8Ps8zLqkzG7gDywaVU0j6Lm1KruBe1YfI1HP4jDpQeFjbzyuWZhJJMRzp7e1v5ir5o1Euo4QX_oESU1pw9LVkvxlb68LVDtNpuOTmyTNVRePkK-uQy61vJG0yGrzaSMswBDiD6IBIa6ltb1noqfMOON-csDt_OZbCx88TjWgXYA2wBJ2weM7uJHspDytFDgnSUn3s30cZJVJTNxmlBzIHhpybq6RaELQw8uv2buW8G3AxTy-ROO6b03cdD5sS7GsYpn0cnNDZ5Qlg3zKiM7LTvAOFGjT5z5XUbjSX4EB2pIS0PqLtmQdoTlCKJo5ZvgxYKx9BYZXBpR887myBd3MerCZ9i5Aphu35vtcB2M6_YPoSAcHUmsZ2hmzumpznE2bF-59KCBik=w1278-h852-no',
        }
      ],
      handraws: [
        {
          src: '/video/ballMan1.mov',
        },
        {
          src: '/video/ballMan2.mov',
        }
      ],
      bw: [
        {
          src: '/video/midTerm.mov',
        },
        {
          src: '/video/finalProject1.mp4',
        }
      ],
      finals: [
        {
          src: '/video/cheeseMockUp.mp4',
        }
      ]
    }
  },
}
</script>