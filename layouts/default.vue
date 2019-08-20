<template>
  <v-app>
    <v-navigation-drawer
      v-model="drawer"
      fixed
      app
    >
      <v-row align="center" justify="center" class="pa-2">
        <img
          src="~/assets/img/key-logo.png"
          width="100"
          max-width="100"
          >
        </img>
      </v-row>
      <v-card flat class="flex-column text-center">
        <div class="text-break">一般社団法人</div>
        <div class="title font-weight-black">焼き餃子協会</div>
        <div class="font-weight-thin">Yaki Gyoza Association</div>
      </v-card>
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-content>
      <v-container fluid fill-width class="pa-0">
        <nuxt />
      </v-container>
      <v-footer>
        <span>&copy;2018-2019 一般社団法人焼き餃子協会 All Rights Reserved.</span>
      </v-footer>
    </v-content>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      drawer: true,
      fixed: true,
      items: [
        {
          icon: 'mdi-information',
          title: '焼き餃子協会について',
          to: '/#about'
        },
        {
          icon: 'mdi-chat-alert',
          title: 'おしらせ',
          to: '/news'
        },
        {
          icon: 'mdi-account-heart-outline',
          title: '入会案内',
          to: '/entry'
        },
        {
          icon: 'mdi-account-group',
          title: '賛助会員の皆さま',
          to: '/members'
        },
        {
          icon: 'mdi-contact-mail-outline',
          title: 'お問い合わせ',
          to: '/contact'
        }
      ]
    }
  },
  mounted() {
    this.drawer = true;
  }
}
</script>
