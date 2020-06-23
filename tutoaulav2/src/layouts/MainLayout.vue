<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
     
<q-toolbar  class="bg-grey-1 text-black q-pa-md">
           <q-btn flat round dense icon="menu" class="q-mr-sm" />
 <q-avatar>
        <img src="https://cdn.quasar.dev/logo/svg/quasar-logo.svg">
      </q-avatar>
        <q-toolbar-title>
          Tutoaula
        </q-toolbar-title>
          
     <div class="text-bold q-gutter-sm">
       <!-- <div class="text-h6 q-pr-lg"> Contactanos</div> -->
        <q-btn flat color="cyan-9" label="Herramientas" />
        <q-btn flat color="cyan-9" label="Nosotros" />
        <q-btn flat color="cyan-9" label="Contactanos" />
        <q-btn outline color="cyan-9" label="Registro" />
         <q-btn  outline color="pink-4" label="Login" />
     </div>
     
      </q-toolbar>
 
    </q-header>
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import EssentialLink from 'components/EssentialLink'

export default {
  name: 'MainLayout',

  components: {
    EssentialLink
  },

  data () {
    return {
      leftDrawerOpen: false,
      tab: '',
      essentialLinks: [
        {
          title: 'Docs',
          caption: 'quasar.dev',
          icon: 'school',
          link: 'https://quasar.dev'
        },
        {
          title: 'Github',
          caption: 'github.com/quasarframework',
          icon: 'code',
          link: 'https://github.com/quasarframework'
        },
        {
          title: 'Discord Chat Channel',
          caption: 'chat.quasar.dev',
          icon: 'chat',
          link: 'https://chat.quasar.dev'
        },
        {
          title: 'Forum',
          caption: 'forum.quasar.dev',
          icon: 'record_voice_over',
          link: 'https://forum.quasar.dev'
        },
        {
          title: 'Twitter',
          caption: '@quasarframework',
          icon: 'rss_feed',
          link: 'https://twitter.quasar.dev'
        },
        {
          title: 'Facebook',
          caption: '@QuasarFramework',
          icon: 'public',
          link: 'https://facebook.quasar.dev'
        },
        {
          title: 'Quasar Awesome',
          caption: 'Community Quasar projects',
          icon: 'favorite',
          link: 'https://awesome.quasar.dev'
        }
      ]
    }
  }
}
</script>
