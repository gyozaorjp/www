<template>
  <v-layout
    column
    wrap
    justify-center
  >

  <v-parallax
    style="height: 85vh"
    src="/img/key-gyoza.jpg">
    <p class="font-weight-thin gray--text ma-4 text-center overline">美味しい餃子を作る人と食べる人を、もっと増やしたい。</p>
      <v-card
        flat
        light
        width="320px"
        img="/img/cover.png"
        class="px-7 py-9 mx-auto text-center">
        <img src="~/assets/img/key-copy.png" />
        <v-card-text class="white--text">焼き餃子協会は、美味しい餃子を作る人と、美味しく焼く人、美味しく食べる人をつなげる団体です。</v-card-text>
        <v-card-actions>
          <v-col cols="12">
            <div>
              <v-btn href="#about" width="90%" color="primary">焼き餃子協会について</v-btn>
            </div>
            <div class="mt-3">
              <v-btn href="#entry" width="90%" color="primary">入会案内</v-btn>
            </div>
            <div class="mt-3">
              <v-btn href="#contact" width="90%" color="primary">お問い合わせ</v-btn>
            </div>
          </v-col>
        </v-card-actions>
      </v-card>
  </v-parallax>

  <v-parallax id="about" src="/img/about_bg.jpg" height="800">
    <v-card flat color="transparent" class="d-md-flex align-center">
      <v-card dark flat color="rgb(0,0,0, 0.7)" class="mx-8 my-4">
        <v-card-title class="title white--text">
          一般社団法人焼き餃子協会とは
        </v-card-title>
        <v-card-text class="body-2 white--text font-weight-medium">
          <p>世界には餃子（またはそれに似た料理）がさまざまに存在します。<br>日本では焼き餃子が独自に発達し、多様な具による餃子が開発されて、通販で購入できる数だけでも1500種類以上存在します。</p>
          <p>一般社団法人焼き餃子協会は、消費者がより美味しい餃子を楽しむ社会を目指して、餃子や油・調味料そして調理器具などの餃子に関連する業界の発展を支援し、また消費者にも美味しい餃子の焼き方や食べ方などの情報提供を行って参ります。</p>
        </v-card-text>
      </v-card>
      <v-card flat color="transparent" class="text-center mx-8 my-4">
        <img src="~/assets/img/about_img.png" />
      </v-card>
    </v-card>
  </v-parallax>

  <v-card id="entry" color="rgba(229, 211, 184, 0.5)" flat tile class="pt-1">
    <v-card-title class="d-flex justify-center align-center flex-no-wrap">
      <h1 class="display-2">
        <img src="~/assets/img/entry_left.png" alt="" />
        入会のご案内
        <img src="~/assets/img/entry_right.png" alt="" />
      </h1>
    </v-card-title>
    <v-card-text class="text-center body-1 black--text">
      <p>焼き餃子協会は、焼き餃子に関連する業界間に向けて技術・情報支援を通して、<br>餃子を美味しく焼いて食べる日本の文化を世界の人々に楽しんでもらうことを目指しています。</p>
    </v-card-text>
    <v-card-title class="d-block text-center">
      <h2>会員種別</h2>
    </v-card-title>

    <v-card class="ma-4 pa-2">
      <v-card-title>
        <h3>法人会員</h3>
      </v-card-title>
      <v-card-text>
        焼き餃子の品質向上や市場拡大のため、当協会の活動に賛助頂ける企業・団体。
      </v-card-text>
      <v-card class="ma-2 py-2" dark>
        <v-subheader>ご提供サービス</v-subheader>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>会員コミュニティ</v-list-item-title>
            <v-list-item-subtitle>オンライン/オフラインで当協会会員間の情報交換や交流ができる場へご招待いたします。</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>コラボイベント開催</v-list-item-title>
            <v-list-item-subtitle>当協会と共同のイベントを開催するための企画、実施協力を行います。</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>お取り寄せ餃子データベースの閲覧</v-list-item-title>
            <v-list-item-subtitle>当協会が独自に収集した1500件以上のお取り寄せ餃子データベースをご覧頂けます。</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>会員向け情報配信</v-list-item-title>
            <v-list-item-subtitle>餃子への愛情が高い当協会会員向けに、新商品やキャンペーンなどの情報をご案内いたします。</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>会員限定イベント</v-list-item-title>
            <v-list-item-subtitle>会員のみ参加できるイベントをご案内いたします。</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>法人会員リストの掲載</v-list-item-title>
            <v-list-item-subtitle>賛助会員リストに掲載いたします</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>デジタルマーケティングご協力</v-list-item-title>
            <v-list-item-subtitle>お店のホームページやお問い合わせフォーム作成、メールマガジン配信などの計画、実施をお手伝いします（別途料金）</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </v-card>
      <v-card-text>
        法人賛助会費： 10,000円1口〜/年<br>
        賛助会員の年会費は一口以上何口でも承ります。<br>
        法人会員の登録には審査があります。
      </v-card-text>
      <v-card-actions>
        <div class="ma-2">
          <v-btn large color="primary" class="mx-1">法人賛助会員として入会する</v-btn>
          <v-btn large outlined class="mx-1" href="/pdf/sponsor-entry.pdf">ご案内資料をダウンロード</v-btn>
          <v-btn large outlined class="mx-1">相談する</v-btn>
          <v-btn large outlined class="mx-1">賛助会員リスト</v-btn>
        </div>
      </v-card-actions>
    </v-card>

    <v-card class="ma-4 pa-2">
      <v-card-title>
        <h3>個人会員</h3>
      </v-card-title>
      <v-card-text>
        焼き餃子への関心が高く、焼き餃子の品質向上や市場拡大のため、当協会の活動に賛助頂ける個人の方
      </v-card-text>
      <v-card class="ma-2 py-2" dark>
        <v-subheader>ご提供サービス</v-subheader>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>会員コミュニティ</v-list-item-title>
            <v-list-item-subtitle>オンライン/オフラインで当協会会員間の情報交換や交流ができる場へご招待いたします。</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>会員限定イベント</v-list-item-title>
            <v-list-item-subtitle>会員のみ参加できるイベントをご案内いたします。</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>焼き餃子協会メール</v-list-item-title>
            <v-list-item-subtitle>独自のルートから仕入れた新店舗や新商品、割引などの情報、イベントなどのお知らせをお送りします。</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>名刺作成、メールアドレス提供</v-list-item-title>
            <v-list-item-subtitle>焼き餃子協会特製の名刺や、gyoza.orgメールアドレスをご利用頂けます（月会費とは別途料金となります）。</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </v-card>
      <v-card-text>
        個人賛助会費： 324円〜/月
      </v-card-text>
      <v-card-actions>
        <div class="ma-2">
          <v-btn large color="primary" class="mx-1" href="https://yaki-gyoza.stores.jp/items/5c528c8faee1bb700384f98a" target="_blank">個人賛助会員として入会する</v-btn>
          <v-btn large outlined class="mx-1">相談する</v-btn>
        </div>
      </v-card-actions>
    </v-card>

    <v-card class="ma-4 pa-2">
      <v-card-title>
        <h3>特別会員</h3>
      </v-card-title>
      <v-card-text>
        焼き餃子の品質向上や市場拡大のための協力や活動が特に認められる方。
      </v-card-text>
      <v-card class="ma-2 py-2" dark>
        <v-subheader>ご提供サービス</v-subheader>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>表彰</v-list-item-title>
            <v-list-item-subtitle>特に優れた技術や知識を表彰し、多くの人に知ってもらうための努力をします。</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item two-line>
          <v-list-item-content>
            <v-list-item-title>会員コミュニティ</v-list-item-title>
            <v-list-item-subtitle>オンライン/オフラインで当協会会員間の情報交換や交流ができる場へご招待いたします。</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </v-card>
    </v-card>

  </v-card>

  <v-card id="contact" color="rgba(229, 211, 184, 0.5)" flat tile class="pa-4" img="/img/contact_bg.jpg">
    <v-card-title class="d-flex justify-center align-center flex-no-wrap">
      <h1 class="display-2 white--text">
        お問い合わせ・ご相談
      </h1>
    </v-card-title>

  </v-card>

  </v-layout>
</template>

<style scoped lang="scss">
h1.display-2 {
  img {
    height: 5rem;
    vertical-align: middle;
  }
}
.benefits {
  thead th, tbody td {
    text-align: center;
  }
}
</style>
