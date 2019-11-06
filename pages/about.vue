<template>
  <section class="about">
    <h2 class="title">鈴木晃平 / KOHEI SUZUKI</h2>
    <p class="introduction">
      <span class="line-group">
        1992年4月2日、北海道生まれ埼玉育ち、27歳。
      </span>
      <br />
      <span class="line-group">
        2016年、成城大学経済学部卒業後、
      </span>
      <span class="line-group">
        新卒でオフィス家具商社に営業職として入社。
      </span>
      <span class="line-group">
        プログラミングに興味を持ち、
      </span>
      <span class="line-group">
        退職後、職業訓練校にてJavaを学習。
      </span>
      <span class="line-group">
        受講期間中に基本情報技術者資格を取得。
      </span>
      <span class="line-group">
        その後2018年1月にエスワイシステムに入社。
      </span>
      <br />
      <br />
      <span class="line-group">
        現在、荻窪に在住。
      </span>
      <br />
      <span class="line-group">
        趣味は音楽と個人開発で、最近は
      </span>
      <span class="line-group">
        FirebaseとNuxt.jsを主に使用して開発。
      </span>
    </p>
    <h2 class="title">このサイトについて</h2>
    <p class="introduction">
      <span class="line-group">
        このサイトはインフラに「Firebase」という
      </span>
      <span class="line-group">
        Googleのクラウドプラットフォームと
      </span>
      <span class="line-group">
        フロントエンドに「Nuxt.js」という
      </span>
      <span class="line-group">
        Vue.js製のJavaScriptフレームワークを
      </span>
      <span class="line-group">
        使用して構築されている。
      </span>
      <br />
      <span class="line-group">
        ソース管理はGitHubで行われており、
      </span>
      <span class="line-group">
        「CircleCI」というクラウドの
      </span>
      <span class="line-group">
        CI/CDツールを使用し、GitHubに
      </span>
      <span class="line-group">
        ソースがPushされると、自動でFirebaseに
      </span>
      <span class="line-group">
        デプロイを行う仕組みを組んでいる。
      </span>
    </p>
  </section>
</template>

<style lang="scss" scoped>
.about {
  > .title {
    margin-bottom: 24px;
  }
  > .introduction {
    line-height: 2.4rem;
    padding-right: 26vw;
    margin-bottom: 40px;
  }
}

@media screen and (max-width: 560px) {
  .about {
    > .introduction {
      line-height: 2.2rem;
      padding-right: 0;
    }
  }
}
</style>
