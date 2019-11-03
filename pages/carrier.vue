<template>
  <section class="carrier">
    <CarrierCard
      v-for="item in carrierData"
      :key="item.id"
      :title="item.title"
      :period="item.period"
      :overview="item.overview"
      :technology="item.technology"
    ></CarrierCard>
  </section>
</template>

<script>
import CarrierCard from '~/components/page/carrier/CarrierCard.vue'

export default {
  components: {
    CarrierCard
  },
  data() {
    return {
      carrierData: [
        {
          title: '不動産会社 営業向けシステム改修',
          period: 2,
          overview:
            '不動産会社の営業向け顧客管理パッケージソフトの改修案件。' +
            '顧客検索部分の新機能ページの追加を担当。',
          technology: 'PHP/JavaScript/Lumen/jQuery/PostgreSQL/Linux/Vagrant'
        },
        {
          title: 'ポータルサイト データ変換ツール',
          period: 1,
          overview:
            'VBA案件。博物館のポータルサイト改修プロジェクトの一環で、サイトに' +
            '掲示するための資料データを、規格通りに整形するエクセルツールの作成を担当。',
          technology: 'VBA'
        },
        {
          title: '大手複合機メーカー 基幹システム開発テストサポート',
          period: 2,
          overview:
            '大手複合機メーカーの基幹システム改修プロジェクトのテストサポーターとして参画。' +
            'テスト用データ作成や不具合発生時のパッチSQL作成などを担当。',
          technology: 'SQL/OracleDB'
        },
        {
          title: '保証会社 契約管理システムリプレイス',
          period: 9,
          overview:
            '金融関連会社の社内システムのリプレイス案件。Flashで構成されたシステムを' +
            'HTML5/CSS3にて再構成。 主にjQueryによる画面動作部を担当。',
          technology: 'Java/JavaScript/Seasar2/jQuery/SQLServer'
        },
        {
          title: 'サーバーリプレイス',
          period: 7,
          overview:
            '老朽化したサーバーとソフトウェアのリプレイス案件。' +
            '主にバッチ系処理の製造を担当。',
          technology: 'WindowsServer/Java/VBS/JP1/HULFT'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.carrier {
  > .carrier-card {
    margin-bottom: 56px;
  }
}
</style>
