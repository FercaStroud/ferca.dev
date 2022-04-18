<template lang="pug">
.container.text-center.mt-5
  .title.color-gray Portfolio
  h2.color-gray Projects
  .row.mt-5
    article.col-lg-4.col-md-6.col-sm-12.mt-5( v-for="(project,key) in projects" :key="key")
      h3(style="height:80px") {{project.title}}
      figure
        img(:src="project.image")
      p
        a(:href="project.href" target="_blank") {{project.domain}}

      //p(v-for="(tag,i) in project.tags" :key="i")
      //  strong.active.tags {{ '#' + tag}}
      //hr/

</template>

<script lang="ts">
import {defineComponent} from 'vue'

export default defineComponent({
  data() {
    return {
      projects: [
        {
          title: 'Gorilas Online',
          href: 'https://appsgorilasonline.com',
          domain: 'appsgorilasonline.com',
          strike: false,
          image: require('../assets/portfolio/gorilas.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE']
        },
        {
          title: 'Laboratorios Norvet',
          href: 'http://www.norvet.com.mx',
          domain: 'norvet.com.mx',
          strike: false,
          image: require('../assets/portfolio/norvet.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'PHP', 'ECOMMERCE', 'OnlinePayments', 'Dashboard']
        },
        {
          title: 'Q-Restaurant',
          href: 'https://q-restaurant.com/auth/login',
          domain: 'q-restaurant.com',
          strike: false,
          image: require('../assets/portfolio/qrestaurant.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'PHP', 'OnlinePayments', 'Dashboard']
        },
        {
          title: 'OM Human First',
          href: 'http://om-humanfirst.com',
          domain: 'om-humanfirst.com',
          strike: false,
          image: require('../assets/portfolio/omhuman.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'PHP', 'OnlinePayments', 'Dashboard']
        },
        {
          title: 'App iOS/Android Observatorio',
          href: 'http://app.observatoriodelalaguna.org.mx',
          domain: 'app.observatoriodelalaguna.org.mx',
          image: require('../assets/portfolio/appobservatorio.webp'),
          strike: false,
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'PHP', 'AppStorePlayStore', 'AppStore', 'Dashboard']
        },
        {
          title: 'App iOS/Android INAGAVE',
          href: 'https://inagave.com/',
          domain: 'inagave.com',
          image: require('../assets/portfolio/inagave.webp'),
          strike: false,
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'PHP', 'AppStorePlayStore', 'AppStore', 'Dashboard']
        },
        {
          title: 'Panel INAGAVE',
          href: 'https://panel.inagave.com/',
          domain: 'panel.inagave.com',
          image: require('../assets/portfolio/panelinagave.webp'),
          strike: false,
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'PHP', 'AppStorePlayStore', 'AppStore', 'Dashboard']
        },
        {
          title: 'OCIS - Tablero de Evaluación',
          href: 'https://oics.ccilaguna.org.mx/',
          domain: 'oics.ccilaguna.org.mx',
          image: require('../assets/portfolio/oics.webp'),
          strike: false,
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'PHP', 'AppStorePlayStore', 'AppStore', 'Dashboard']
        },
        {
          title: 'iatrikos',
          href: 'https://iatrikos.com/#inicio',
          domain: 'iatrikos.com',
          strike: false,
          image: require('../assets/portfolio/iatrikos.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE']
        },
        {
          title: 'Am Your Accountant',
          href: 'http://amyouraccountant.ca',
          domain: 'amyouraccountant.ca',
          strike: false,
          image: require('../assets/portfolio/amyour.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE']
        },
        {
          title: 'AVANI',
          href: 'http://avanimx.com.mx/',
          domain: 'avanimx.com.mx',
          image: require('../assets/portfolio/avani.webp'),
          strike: false,
          tags: ['CSS', 'HTML', 'JS', 'VUE']
        },
        {
          title: 'Ludum MX',
          href: 'http://ludummx.com/',
          domain: 'ludummx.com',
          image: require('../assets/portfolio/ludum.webp'),
          strike: false,
          tags: ['CSS', 'HTML', 'JS', 'VUE']
        },
        {
          title: 'Enmedio Asociados',
          href: 'https://enmedioasociados.com/',
          domain: 'enmedioasociados.com',
          image: require('../assets/portfolio/enmedio.webp'),
          strike: false,
          tags: ['CSS', 'HTML', 'JS', 'VUE']
        },
        {
          title: 'Adolfo R. Silva',
          href: 'https://www.adolforsilva.com/',
          domain: 'adolforsilva.com',
          image: require('../assets/portfolio/nodisponible.webp'),
          strike: false,
          tags: ['CSS', 'HTML', 'JS', 'VUE']
        },
        {
          title: 'ARS Consultoría Política',
          href: 'https://arsconsultoriapolitica.com/',
          domain: 'arsconsultoriapolitica.com',
          image: require('../assets/portfolio/ars.webp'),
          strike: false,
          tags: ['CSS', 'HTML', 'JS', 'VUE']
        },
        {
          title: 'Casas BIOS',
          href: 'http://casasbios.com.mx/',
          domain: 'casasbios.com.mx',
          image: require('../assets/portfolio/bios.webp'),
          strike: false,
          tags: ['CSS', 'HTML', 'JS', 'VUE']
        },
        {
          title: 'Kingans',
          href: '#',
          domain: 'kingans.com',
          strike: false,
          image: require('../assets/portfolio/kingans.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'FirstVersion']
        },
        {
          title: 'Argi Residencias',
          href: '#',
          domain: 'argiresidencias.com',
          image: require('../assets/portfolio/nodisponible.webp'),
          strike: true,
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
        {
          title: 'ECO3',
          href: '#',
          domain: 'eco3.com.mx',
          strike: true,
          image: require('../assets/portfolio/nodisponible.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
        {
          title: 'Bosque y Lago',
          href: '#',
          domain: 'bosqueylago.com',
          strike: true,
          image: require('../assets/portfolio/nodisponible.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
        {
          title: 'Venta de Terrenos Laguna',
          href: '#',
          image: require('../assets/portfolio/nodisponible.webp'),
          domain: 'ventadeterrenoslaguna.com',
          strike: true,
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
        {
          title: 'Vende tu Home',
          href: '#',
          domain: 'vendetuhome.com',
          strike: true,
          image: require('../assets/portfolio/nodisponible.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
        {
          title: 'Mediciones MX',
          href: '#',
          domain: 'medicionesmx.com',
          strike: true,
          image: require('../assets/portfolio/nodisponible.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
        {
          title: 'Jorge Zermeño',
          href: '#',
          domain: 'jorgezermeno.com',
          strike: true,
          image: require('../assets/portfolio/nodisponible.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
        {
          title: 'The Happy Lesson',
          href: '#',
          domain: 'thehappylesson.com',
          strike: true,
          image: require('../assets/portfolio/nodisponible.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
        {
          title: 'SLAK',
          href: '#',
          domain: 'slak.mx',
          strike: false,
          image: require('../assets/portfolio/nodisponible.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE']
        },
        {
          title: 'Innvalo',
          href: '#',
          domain: 'innvalo.com',
          strike: true,
          image: require('../assets/portfolio/nodisponible.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
        {
          title: 'MR. Dunks',
          href: '#',
          domain: 'mrdunks.com',
          strike: true,
          image: require('../assets/portfolio/nodisponible.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
        {
          title: 'Canteras Portofino',
          href: '#',
          domain: 'canterasportofino.com',
          strike: true,
          image: require('../assets/portfolio/nodisponible.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
        {
          title: 'Tenlasa',
          href: '#',
          domain: 'tenlasa.com',
          strike: true,
          image: require('../assets/portfolio/nodisponible.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
        {
          title: 'Grupo Kingans',
          href: '#',
          domain: 'grupokingans.com',
          strike: false,
          image: require('../assets/portfolio/nodisponible.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'FirstVersion']
        },
        {
          title: 'MSana',
          href: '#',
          domain: 'msana.mx',
          image: require('../assets/portfolio/nodisponible.webp'),
          strike: true,
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
        {
          title: 'Compañía Transforma',
          href: '#',
          domain: 'companiatransforma.com',
          strike: false,
          image: require('../assets/portfolio/nodisponible.webp'),
          tags: ['CSS', 'HTML', 'JS', 'VUE', 'Archived']
        },
      ]
    }
  },
  mounted() {
  },
  methods: {}
})


</script>


<style scoped lang="scss">


</style>
