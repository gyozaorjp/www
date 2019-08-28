<template>
  <v-app>

    <v-navigation-drawer
      app
      v-model="drawer">
      <v-row align="center" justify="center" class="pa-2">
        <nuxtLink to="/">
          <img src="~/assets/img/key-logo.png" width="100px" max-width="100px" />
        </nuxtLink>
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
          :href="item.href"
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

    <v-app-bar app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title class="title font-weight-thin">
        <v-btn text depressed href="/">一般社団法人 焼き餃子協会</v-btn>
      </v-toolbar-title>
    </v-app-bar>

    <v-content>
      <v-container fluid class="pa-0">
        <nuxt />
      </v-container>
      <v-footer>
        <p class="font-weight-light">
          <span>&copy;2018-2019&nbsp;</span>
          <a href="https://www.gyoza.or.jp/">一般社団法人焼き餃子協会</a>
          <span>&nbsp;All Rights Reserved.</span>
        </p>
      </v-footer>
    </v-content>

  </v-app>
</template>

<script>
export default {
  data () {
    return {
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-information',
          title: '焼き餃子協会について',
          href: '/#about'
        },
        {
          icon: 'mdi-chat-alert',
          title: 'おしらせ',
          to: '/news'
        },
        {
          icon: 'mdi-account-heart-outline',
          title: '入会案内',
          href: '/#entry'
        },
        {
          icon: 'mdi-account-group',
          title: '賛助会員の皆さま',
          to: '/members'
        },
        {
          icon: 'mdi-contact-mail-outline',
          title: 'お問い合わせ',
          href: '/#contact'
        }
      ]
    }
  }
}
</script>
<style scoped>
.v-application {
  font-family: 'Roboto', 'Noto Sans JP', sans-serif;
}
.v-footer a {
  text-decoration: none;
  color: #000;
}
</style>
