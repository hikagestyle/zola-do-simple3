# まえがき

Zola（静的サイトジェネレーター）のテーマ。

個人的なファイル一式。

修正や加工ほか、ご利用は自己責任で。


## 環境

- x230(Lenovo ThinkPad)
- LinuxMint 20.2


## 補足

サクッと使う個人的な用途で小規模を想定。

blogフォルダへ投稿を詰め込んで、タグで仕分けるイメージ。

Zolaで個人的に使うシンプルなテーマ。

短時間で作ったので、大雑把にやっつけです。

公開日:2022-02-06


### 2022-08-20（修正）

- templates/blog-page.html
	- v0.15.3,v0.16.0,v0.16.1で記事の前後ナビ対策


## 基本的な仕様

ドメイン直下、サブディレクトリでも、とりあえず使えるはず。（config.tomlのbase_urlによる）

- Zola v0.15.2
- pure.css
- config.toml
	- base_url（最後のスラッシュ無し）
- カテゴリー無し
- タグ（taxonomies）有効
	- 日本語のタグ付けは、zolaの仕様で自動的に英数字へ変換される
- ページ送り:デフォルトで10件ごと
	- content/blog
- タグのページ送り:デフォルトで5件ごと
	- config.tomlから変更可
	- テンプレートの場所:templates/tags/single.html
- 投稿のURL=ファイル名（.mdファイル）
- 固定ページのテンプレート（デフォルト:日付表示なし）
	- 日付表示はコメントアウト
	- templates/static.html
- メニューページ（固定ページ）


## 完成イメージ

デモサイト: https://zola-do-simple3.netlify.app/


## 公式サイト

- [Zola](https://www.getzola.org/)
- [Pure](https://purecss.io/)

