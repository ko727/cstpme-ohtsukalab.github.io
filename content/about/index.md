---
title: "About"
type: page
share: false
---
<style>
.article-container, main .container, .prose {
  max-width: 1200px !important; /* お好みの横幅（例: 1000px, 1100px, 1200pxなど）に指定 */
}
</style>
<div style="max-width: 1200px; margin: 0 auto; color: #cbd5e1; line-height: 1.9;">

<!-- 1. トップ見出しとリード文 -->
<h2 style="color: #ffffff; border-bottom: 2px solid #334155; padding-bottom: 12px; margin-top: 20px; font-size: 1.6rem;">
  構造解析とロボット技術で機械システムを安全にする
</h2>

<p style="font-size: 1.05rem; margin-top: 20px;">
  科学技術の進歩に伴い，私たちの周りにはロボット化された輸送システムや機械システム，高機能化された都市空間が発達してきましたが，同時に私たちが創りだした様々な機械機器や工作物によって人々の命が奪われる事故が社会問題となっています．
</p>

<p style="font-size: 1.05rem;">
  構造力学研究室では，<strong style="color: #ffffff;">「安全に配慮した機械構造設計」</strong>と<strong style="color: #ffffff;">「安全を護るための機械システム開発」</strong>を目的として，衝突安全性能向上のため材料設計，スポーツのトレーニング支援システムの開発，インフラ構造のメンテナンスロボット開発，ゼロエミッション宇宙往還機（宇宙エレベータ）の開発など，社会の要求に基づいた機械システムの開発・設計を行っています．そのため，材料力学（機械系）の知識を基本として，非破壊検査やヘルスモニタリングのための計測技術（電気・電子系），データの可視化や自動化ロボットのシステム開発のためのプログラミング（情報系）の幅広い分野の知識・技術を用いています．
</p>
</div>

<!-- 2. 研究室の成り立ち（新規追加部分） -->
<div style="background-color: rgba(30, 41, 59, 0.5); border: 1px solid #334155; padding: 24px; border-radius: 8px; margin: 40px 0;">
  <h3 style="color: #ffffff; font-size: 1.25rem; margin-top: 0; margin-bottom: 16px; display: flex; align-items: center;">
    <span style="display: inline-block; width: 4px; height: 1.25rem; background-color: #38bdf8; margin-right: 12px; border-radius: 2px;"></span>
    研究室の成り立ちと歩み
  </h3>
  <p style="margin-bottom: 12px;">
    本研究室は，青木義男 先生が長年牽引されてきた「構造力学研究室」の系譜を引き，同研究室の卒業生でもある大塚（現指導教員）のもと，<strong style="color: #ffffff;">2025年4月1日より新体制としてスタート</strong>しました．
  </p>
  <p style="margin-bottom: 0;">
    強化繊維プラスチック（FRP）の力学特性の解明，ゼロエミッションを目指す宇宙エレベータ構想，そしてインフラの未来を守る構造ヘルスモニタリング技術など，これまでに培われた中核的な研究プロジェクトを継承しつつ，次世代の機械システム開発へと発展させています．
  </p>
</div>

<!-- 📷 自動フェードスライドショー -->
<div style="position: relative; width: 100%; aspect-ratio: 16 / 9; max-height: 600px; overflow: hidden;">
  
  <!-- 画像の指定（枚数に合わせて増減可能です） -->
  <img class="about-slide" src="/media/about_sports1.jpg" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; object-fit: contain; object-position: top; opacity: 1; transition: opacity 1.5s ease-in-out;">
  <img class="about-slide" src="/media/about_sports2.jpg" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; object-fit: contain; object-position: top; opacity: 0; transition: opacity 1.5s ease-in-out;">
  <img class="about-slide" src="/media/about_frp1.jpg" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; object-fit: contain; object-position: top; opacity: 0; transition: opacity 1.5s ease-in-out;">
  <img class="about-slide" src="/media/about_frp2.jpg" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; object-fit: contain; object-position: top; opacity: 0; transition: opacity 1.5s ease-in-out;">
  <img class="about-slide" src="/media/about_wire1.jpg" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; object-fit: contain; object-position: top; opacity: 0; transition: opacity 1.5s ease-in-out;">
  <img class="about-slide" src="/media/about_wire2.jpg" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; object-fit: contain; object-position: top; opacity: 0; transition: opacity 1.5s ease-in-out;">
  <img class="about-slide" src="/media/about_uele1.jpg" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; object-fit: contain; object-position: top; opacity: 0; transition: opacity 1.5s ease-in-out;">
  <img class="about-slide" src="/media/about_uele2.jpg" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; object-fit: contain; object-position: top; opacity: 0; transition: opacity 1.5s ease-in-out;">

</div>

<!-- スライドを動かすプログラム -->
<script>
document.addEventListener('DOMContentLoaded', function() {
  const slides = document.querySelectorAll('.about-slide');
  let current = 0;
  if(slides.length > 1) {
    setInterval(() => {
      slides[current].style.opacity = '0'; // 現在の画像を透明にする
      current = (current + 1) % slides.length; // 次の画像の番号を計算
      slides[current].style.opacity = '1'; // 次の画像を表示する
    }, 4500); // 4500ミリ秒（4.5秒）ごとに切り替わります
  }
});
</script>
<!-- 📷 追加ここまで -->

<!-- 3. 主な研究プロジェクト -->
<hr style="border: none; border-top: 1px solid #334155; margin: 40px 0;">

<h3 style="color: #ffffff; font-size: 1.3rem; margin-bottom: 20px;">主な研究プロジェクト</h3>

<!-- 💡 ここを grid から flex の縦並び（column）に変更しました -->
<div style="display: flex; flex-direction: column; gap: 20px; margin-bottom: 40px;">

  <!-- プロジェクト1：スポーツ器具 -->
  <a href="/research/#sports" style="text-decoration: none; display: block; background-color: #1e293b; padding: 20px; border-radius: 6px; border-left: 4px solid #3b82f6; transition: background-color 0.3s;" onmouseover="this.style.backgroundColor='#334155'" onmouseout="this.style.backgroundColor='#1e293b'">
    <h4 style="color: #ffffff; margin-top: 0; font-size: 1.1rem; display: flex; align-items: center; justify-content: space-between;">
      01. スポーツ器具によるデータ収集・分析
      <span style="color: #3b82f6; font-size: 1.2rem;">→</span>
    </h4>
    <p style="margin: 0; font-size: 0.95rem; color: #94a3b8;">スポーツ器具によるパフォーマンス向上と事故予防を目的とし，器具を用いたデータ収集・分析技術</p>
  </a>

  <!-- プロジェクト2：強化繊維プラスチック -->
  <a href="/research/#frp" style="text-decoration: none; display: block; background-color: #1e293b; padding: 20px; border-radius: 6px; border-left: 4px solid #3b82f6; transition: background-color 0.3s;" onmouseover="this.style.backgroundColor='#334155'" onmouseout="this.style.backgroundColor='#1e293b'">
    <h4 style="color: #ffffff; margin-top: 0; font-size: 1.1rem; display: flex; align-items: center; justify-content: space-between;">
      02. 強化繊維プラスチックの力学特性
      <span style="color: #3b82f6; font-size: 1.2rem;">→</span>
    </h4>
    <p style="margin: 0; font-size: 0.95rem; color: #94a3b8;">軽量・高強度材料である強化繊維プラスチック（FRP）の複雑な力学特性を解明</p>
  </a>

  <!-- プロジェクト3：ワイヤロープ -->
  <a href="/research/#wire-rope" style="text-decoration: none; display: block; background-color: #1e293b; padding: 20px; border-radius: 6px; border-left: 4px solid #3b82f6; transition: background-color 0.3s;" onmouseover="this.style.backgroundColor='#334155'" onmouseout="this.style.backgroundColor='#1e293b'">
    <h4 style="color: #ffffff; margin-top: 0; font-size: 1.1rem; display: flex; align-items: center; justify-content: space-between;">
      03. ワイヤロープの非破壊検査
      <span style="color: #3b82f6; font-size: 1.2rem;">→</span>
    </h4>
    <p style="margin: 0; font-size: 0.95rem; color: #94a3b8;">社会インフラの安全を維持する，内部損傷のリアルタイム検知とヘルスモニタリング技術</p>
  </a>

  <!-- プロジェクト4：宇宙エレベータ -->
  <a href="/research/#space-elevator" style="text-decoration: none; display: block; background-color: #1e293b; padding: 20px; border-radius: 6px; border-left: 4px solid #3b82f6; transition: background-color 0.3s;" onmouseover="this.style.backgroundColor='#334155'" onmouseout="this.style.backgroundColor='#1e293b'">
    <h4 style="color: #ffffff; margin-top: 0; font-size: 1.1rem; display: flex; align-items: center; justify-content: space-between;">
      04. 宇宙エレベータのクライマロボット
      <span style="color: #3b82f6; font-size: 1.2rem;">→</span>
    </h4>
    <p style="margin: 0; font-size: 0.95rem; color: #94a3b8;">環境負荷ゼロの宇宙往還を実現する，超高高度昇降ロボットの構造設計と制御システム</p>
  </a>

</div>