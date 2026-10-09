---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: |
        <span style="color: #ffffff; white-space: nowrap;">構造力学研究室</span>
      text: |
        <div style="color: #94a3b8; max-width: 750px; margin: 0 auto; line-height: 1.8; font-size: 1.1rem;">
          <strong style="color: #ffffff;">構造解析とロボット技術で機械システムを安全にする</strong>
        </div>

        <!-- 💡 HTMLによるカスタムボタン -->
        <div style="margin-top: 20px;">
          <a href="/about/" style="display: inline-block; padding: 6px 16px; font-size: 0.85rem; color: #9797a5; border: 0px solid #0a0a0a; border-radius: 4px; text-decoration: none; font-weight: bold; background-color: rgba(7, 11, 14, 0.54); transition: all 0.3s;">
            About us >
          </a>
        </div>

    design:
      is_dark: true
      background:
        image:
          filename: uele.jpg
          filters:
            brightness: 0.25 # 数値を小さくして背景写真をぐっと暗く落とします
      spacing:
        padding: ['200px', '0', '200px', '0'] # 上下余白を広く取ってシックに見せる
  
  - block: collection
    id: news          # メニュー等で参照用ID
    content:
      title: '<span style="color: #ffffff;">News</span>'
      filters:
        folders:
          - news      # お知らせ記事が入っているフォルダ名（content/news/）
      count: 5        # 💡 ここで Home 画面に表示する最新件数を 5 件に制限します[cite: 1]
      
      # 「過去の記事一覧を見る」ボタンを設置する場合（任意）
      archive:
        enable: true
        text: '過去の一覧を見る'
        link: '/news/' # 全件一覧ページへのリンク
    design:
      view: compact   # リスト表示（日付とタイトルのみのスッキリした配置）[cite: 1, 2]
      is_dark: true
      background:
        color: '#121217d9'


---
