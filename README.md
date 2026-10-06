# ICU Masterclass

聖路加国際病院 集中治療科の教育資料（Web版＋PDF版）を GitHub Pages で公開するリポジトリ。
**リンクを知っている人だけが閲覧できる**運用（`noindex` ＋ `robots.txt` で検索エンジンには載せない）。

- 入口: https://hiro-oka.github.io/icu-masterclass/

## 収録

| # | 資料 | Web | PDF |
|---|---|---|---|
| 01 | NIV（非侵襲的換気）実戦管理ガイド | [resident-niv/](https://hiro-oka.github.io/icu-masterclass/resident-niv/) | [PDF](https://hiro-oka.github.io/icu-masterclass/resident-niv/resident-niv.pdf) |
| 02 | HFNC（高流量鼻カニュラ） | [resident-hfnc/](https://hiro-oka.github.io/icu-masterclass/resident-hfnc/) | [PDF](https://hiro-oka.github.io/icu-masterclass/resident-hfnc/resident-hfnc.pdf) |
| 03 | DKA・HHS（高血糖緊急症） | [resident-dka-hhs/](https://hiro-oka.github.io/icu-masterclass/resident-dka-hhs/) | [PDF](https://hiro-oka.github.io/icu-masterclass/resident-dka-hhs/resident-dka-hhs.pdf) |
| 04 | 正常血糖DKA（euglycemic DKA） | [resident-edka/](https://hiro-oka.github.io/icu-masterclass/resident-edka/) | [PDF](https://hiro-oka.github.io/icu-masterclass/resident-edka/resident-edka.pdf) |

## ファイル構成

```
index.html                                 入口（資料一覧）
niv/index.html                             旧NIV版。resident-niv/ への転送ページ（2026-09-28 一本化）
robots.txt                                 検索エンジン除外
```

## 更新のしかた

各ページは院内の正本HTMLから生成します（resident-niv・resident-hfnc などは `masterclass_share.py --src <正本> --slug <slug>` で HTML と PDF を作り、自動で push）。このリポジトリのHTMLを直接編集しないでください。

## 出典と注意

教育目的の資料です。数値にはできるだけ出典を付けていますが、臨床判断は患者背景と各施設のプロトコルを優先してください。

