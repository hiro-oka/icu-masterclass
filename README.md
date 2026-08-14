# ICU Masterclass

聖路加国際病院 集中治療科の教育資料（Web版＋PDF版）を GitHub Pages で公開するリポジトリ。
**リンクを知っている人だけが閲覧できる**運用（`noindex` ＋ `robots.txt` で検索エンジンには載せない）。

- 入口: https://hiro-oka.github.io/icu-masterclass/

## 収録

| # | 資料 | Web | PDF |
|---|---|---|---|
| 01 | NIV / NPPV in the ICU | [niv/](https://hiro-oka.github.io/icu-masterclass/niv/) | [PDF](https://hiro-oka.github.io/icu-masterclass/niv/NIV_NPPV_ICU_Masterclass_2026.pdf) |

## NIV / NPPV の構成

1. NIV / NPPVとは（定義・EPAP/IPAP・PS・生理・HFNC/IMVとの位置づけ）
2. 適応と禁忌（病態別の一手・判断ゲート・failure plan）
3. 長所と短所
4. マスクの違い（鼻・鼻口・トータルフェイス・ヘルメット・マウスピース）
5. モードの違い（CPAP / S / T / S-T / PC / AVAPS・trigger・cycling・rise time）
6. リークの扱い（意図的リークと意図しないリーク・回路とマスクの組み合わせ・対応の順番）
7. 管理上の注意点（装着手順・皮膚障害・加湿・胃膨満・鎮静・監視・HACOR計算機・当直チェックリスト・weaning）
8. エビデンス（ATS 2026・病態別・ARDS・P‑SILI・PEEP ceiling・helmet・挿管タイミング）

## ファイル構成

```
index.html                                 入口（資料一覧）
niv/index.html                             NIV Web版（単一ファイル・オフライン動作）
niv/NIV_NPPV_ICU_Masterclass_2026.pdf      NIV PDF版（A4 / 28ページ）
robots.txt                                 検索エンジン除外
```

Web版は外部ライブラリに依存しない単一ファイル。ダウンロードしてローカルでも開けます。

## 更新のしかた

1. `niv/index.html` を編集
2. PDFを作り直す

```bash
chrome-headless-shell --headless --no-pdf-header-footer --virtual-time-budget=10000 \
  --print-to-pdf=niv/NIV_NPPV_ICU_Masterclass_2026.pdf "file://$PWD/niv/index.html"
```

3. `git add -A && git commit && git push`（1〜2分でPagesに反映）

## 出典と注意

OpenEvidence の回答と引用文献を統合し、臨床判断の順序に再構成したもの。
「マスクの違い」「モードの違い」「リークの扱い」「管理上の注意点」の各章には、掲載文献に直接対応しない標準的な実務知識・機器の一般原則を含みます（機種ごとの仕様は各施設の取扱説明書とprotocolを優先）。

> **教育目的の資料です。** 患者個別の挿管判断や施設 protocol の代替ではありません。挿管 timing に関する観察研究は association として解釈してください。図はすべて本資料のために作図した模式図です。

---

聖路加国際病院 集中治療科 · ICU Masterclass 2026
