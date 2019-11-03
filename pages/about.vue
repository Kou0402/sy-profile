<template>
  <section class="about">
    <h2 class="name">鈴木晃平 / KOHEI SUZUKI</h2>
    <p class="introduction">
      1992年4月2日、北海道生まれ埼玉育ち、27歳。<br />
      2016年、成城大学経済学部卒業後、<br />
      新卒でオフィス家具商社の営業職として入社。<br />
      プログラミングに興味を持ち、退職後、職業訓練校にてJavaを学習。<br />
      その後2018年1月にエスワイシステムに入社。<br />
      <br />
      現在、荻窪に在住。<br />
      趣味は音楽と個人開発で、最近はFirebaseとNuxt.jsを主に使用して開発。<br />
      このサイトもFirebaseとNuxt.jsを使用しており<br />
      また、GitHubとCircleCIの連携による自動デプロイ構成となっている。
    </p>
  </section>
</template>

<style lang="scss" scoped>
.about {
  > .name {
    font-weight: 500;
    margin-bottom: 24px;
  }
  > .introduction {
    line-height: 2.4rem;
  }
}
</style>
