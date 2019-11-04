<template>
  <section class="about">
    <h2 class="name">鈴木晃平 / KOHEI SUZUKI</h2>
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
        その後2018年1月にエスワイシステムに入社。
      </span>
    </p>
    <p class="introduction">
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
      <span class="line-group">
        このサイトもFirebaseとNuxt.jsで
      </span>
      <span class="line-group">
        構成されている。
      </span>
    </p>
  </section>
</template>

<style lang="scss" scoped>
.about {
  > .name {
    margin-bottom: 24px;
  }
  > .introduction {
    line-height: 2.4rem;
    padding-right: 26vw;
  }
}

@media screen and (max-width: 560px) {
  .about {
    > .name {
      margin-bottom: 24px;
    }
  }
}
</style>
