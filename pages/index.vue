<template>
  <v-layout
    column
    justify-center
    align-center
  >
  <v-card
    flat
    tile
    width="100vw"
    height="700px"
    img="/img/key-gyoza.jpg">
    <p class="font-weight-thin white--text ma-4 text-center overline">美味しい餃子を作る人と食べる人を、もっと増やしたい。</p>
    <v-overlay
      absolute
      opacity="0">
      <v-card
        light
        width="320px"
        img="/img/cover.png"
        class="px-7 py-9 text-center">
        <img src="~/assets/img/key-copy.png" />
        <v-card-text class="white--text">焼き餃子協会は、美味しい餃子を作る人と、美味しく焼く人、美味しく食べる人をつなげる団体です。</v-card-text>
        <v-card-actions>
          <v-col cols="12">
            <div>
              <v-btn href="/#about" width="90%" color="primary">焼き餃子協会について</v-btn>
            </div>
            <div class="mt-3">
              <v-btn href="/#entry" width="90%" color="primary">入会案内</v-btn>
            </div>
          </v-col>
        </v-card-actions>
      </v-card>
    </v-overlay>
  </v-card>

  <v-card id="about"
    flat
    tile
    img="/img/about_bg.jpg">
    <v-card  color="rgb(0,0,0,0.4)">
      <v-row justify="center" align="center">
        <v-col md="5" offset-md="1" sm="12">
          <v-card color="rgb(0,0,0, 0.3)">
            <v-card-title class="headline white--text">
              一般社団法人焼き餃子協会とは
            </v-card-title>
            <v-card-text class="body-1 white--text font-weight-medium">
              <p>世界には餃子（またはそれに似た料理）がさまざまに存在します。<br>日本では焼き餃子が独自に発達し、多様な具による餃子が開発されて、通販で購入できる数だけでも1500種類以上存在します。</p>
              <p>一般社団法人焼き餃子協会は、消費者がより美味しい餃子を楽しむ社会を目指して、餃子や油・調味料そして調理器具などの餃子に関連する業界の発展を支援し、また消費者にも美味しい餃子の焼き方や食べ方などの情報提供を行って参ります。</p>
            </v-card-text>
          </v-card>
        </v-col>
        <v-col md="6" sm="12">
          <v-card color="transparent" class="text-center">
            <img src="~/assets/img/about_img.png" />
          </v-card>
        </v-col>
      </v-row>
    </v-card>
  </v-card>

  <v-card id="entry" flat tile>
    <v-card-title>
      入会のご案内
    </v-card-title>
  </v-card>

  </v-layout>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    VuetifyLogo
  }
}
</script>
