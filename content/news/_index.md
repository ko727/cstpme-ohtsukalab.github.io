---
title: "News"
type: landing

sections:
  # 💡 デザイン・横幅・余白の調整
  - block: markdown
    content:
      text: |
        <style>
        /* 1. 外枠コンテナを1200pxに拡張 */
        .article-container, main .container, .prose, .container-fluid, .site-content, .wg-collection .container {
          max-width: 1000px !important;
          width: 100% !important;
        }
        
        /* 2. 💡 表示幅が変わらない原因：Hugo Blox内部のカラム幅制限（col-lg-8等）を100%に強制解除 */
        .wg-collection .row,
        .wg-collection [class*="col-"] {
          max-width: 100% !important;
          width: 100% !important;
          flex: 0 0 100% !important;
        }
        
        /* 3. 各記事カードを1200px（親要素いっぱい）まで広げる */
        .wg-collection .stream-item,
        .wg-collection .media-stream {
          width: 100% !important;
          max-width: 1200px !important;
          box-sizing: border-box !important;
        }
        
        /* 上下の余白リセット */
        section.wg-markdown, section.wg-collection, .home-section {
          padding-top: 0 !important;
          padding-bottom: 0 !important;
          margin-top: 0 !important;
        }
        
        /* News Archive（見出し）を中央揃え */
        .wg-collection .section-heading {
          text-align: center !important;
          margin-top: 40px !important;
          margin-bottom: 24px !important;
        }
        .wg-collection .section-heading h1 {
          color: #ffffff !important;
          font-size: 1.8rem !important;
          border-bottom: none !important;
        }
        
        /* ニュース記事のデザイン「枠なし＋左太線」 */
        .stream-item {
          background-color: transparent !important;
          border: none !important;
          border-left: 4px solid #3b82f6 !important;
          border-radius: 0 !important;
          padding: 12px 0 12px 20px !important;
          margin-bottom: 30px !important;
          text-align: left !important;
          transition: border-color 0.3s ease !important;
        }
        .stream-item:hover {
          background-color: transparent !important;
          border-left-color: #38bdf8 !important;
        }
        /* タイトルと日付「以外」の要素を非表示にする */
        .article-style, 
        .stream-item .article-style,
        .stream-item .btn-links,
        .stream-item .article-tags,
        .stream-item img {
          display: none !important;
        }


        /* タイトルと日付の配色 */
        .article-title {
          margin-bottom: 8px !important;
        }
        .article-title a {
          color: #ffffff !important;
          font-weight: bold !important;
          font-size: 1.25rem !important;
        }
        .article-title a:hover {
          color: #38bdf8 !important;
        }
        
        /* 日付メタ情報の装飾 */
        .stream-meta, .article-metadata {
          color: #94a3b8 !important;
          font-size: 0.95rem !important;
        }
        </style>
    design:
      spacing:
        padding: ['0', '0', '0', '0']

  # 💡 自動記事一覧
  - block: collection
    content:
      title: "News Archive"
      subtitle: "過去のお知らせ・更新情報一覧"
      filters:
        folders:
          - news
    design:
      view: compact
      is_dark: true
      background:
        color: 'transparent'
      spacing:
        padding: ['0', '0', '0', '0']
---