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
          <a href="https://ko727.github.io/cstpme-ohtsukalab.github.io/about/" style="display: inline-block; padding: 6px 16px; font-size: 0.85rem; color: #9797a5; border: 0px solid #0a0a0a; border-radius: 4px; text-decoration: none; font-weight: bold; background-color: rgba(7, 11, 14, 0.54); transition: all 0.3s;">
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
  
  # 💡 お知らせ（Recent News）セクション
  - block: collection
    id: news
    content:
      title: News
      filters:
        folders:
          - news
        count: 5  # トップページに表示する件数
      text: |
        <style>
        /* ホーム画面のNewsブロック全体の余白や位置を調整 */
        #news {
          max-width: 1100px !important;
          margin: 0 auto !important;
          padding-top: 40px !important;
          padding-bottom: 40px !important;
        }
        
        /* ニュース記事カードのデザインを「枠なし＋左太線」に変更 */
        #news .stream-item {
          background-color: transparent !important;
          border: none !important;
          border-left: 4px solid #3b82f6 !important;
          border-radius: 0 !important;
          padding: 8px 0 8px 16px !important; /* スッキリ見せるため少し余白を狭く */
          margin-bottom: 24px !important;
          text-align: left !important;
          transition: border-color 0.3s ease !important;
        }
        #news .stream-item:hover {
          background-color: transparent !important;
          border-left-color: #38bdf8 !important;
        }
        
        /* 🌟 タイトルと日付「以外」の要素（抜粋文、続きを読むボタン、タグなど）を非表示にする */
        #news .article-style, 
        #news .stream-item .article-style,
        #news .stream-item .btn-links,
        #news .stream-item .article-tags {
          display: none !important;
        }
        
        /* タイトルと日付の配色・配置調整 */
        #news .article-title {
          margin-top: 0 !important;
          margin-bottom: 4px !important; /* タイトルと日付の間隔を詰める */
        }
        #news .article-title a {
          color: #ffffff !important;
          font-weight: bold !important;
          font-size: 1.15rem !important; /* 少し控えめなサイズに調整 */
        }
        #news .article-title a:hover {
          color: #38bdf8 !important;
        }
        
        /* 日付の装飾 */
        #news .stream-meta, #news .article-metadata {
          color: #94a3b8 !important;
          font-size: 0.9rem !important;
          margin-bottom: 0 !important;
        }
        </style>
    design:
      view: compact
      is_dark: true
      background:
        color: 'transparent'


---
