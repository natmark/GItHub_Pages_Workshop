<!-- $theme: gaia -->
<!--page_number : true-->
<!-- template : gaia -->

# GitHub Pages Workshop

## 2017 / 02 / 02

---

<!-- template : normal -->

## <font face="arial">自己紹介</font>

<hr>

<div style="float:left;">
<br \>
Presenter : 佐藤敦也

<a href="http://natmark.github.io">http://natmark.github.io</a>

- 公立はこだて未来大学
知能システムコース 2年
- iOSエンジニア
</div>
<p><img alt="repo" src="https://scontent.xx.fbcdn.net/v/t1.0-9/11401172_1599957510266613_1959919015970162703_n.jpg?oh=5a8bf0f0f181d26469afcabae290f8de&oe=58C4FAF3" style="display:block;margin-left:auto" width="200px" /></p>  
<br \>

---

## <font face="arial">注意事項</font>

- 本ワークショップではGit及びGitHubの大部分の説明を省略します。
- 後半で、演習を行いますが、複数人開発については触れないためmasterブランチ一本で作業します。
- 発表者はPagesエバンジェリストではありません。
- 本ワークショップはFIVEBOX合同会社のIT人材育成事業の一環として行っております。

---

## <font face="arial">FIVEBOX合同会社</font>

http://fivebox.org/
&nbsp;

- スマートフォンアプリ開発 / 人材育成事業 / 民泊事業
&nbsp;


- 現在社員6名(うち5名が未来大学のアルバイト)
- エンジニア4名、デザイナー1名 (+ インターン2名)

---

![](/Users/AtsuyaSato/Desktop/Workshop/Assets/16113156_330411674019225_1158213924869942903_o.jpg)

---
<!-- template : gaia -->
# GitHub Pages Workshop

---
<!-- template : normal -->
## <font face="arial">GitHubとは</font>

<hr>

- エンジニアにとって欠かせないツールの一つ

- ソフトウェア開発プロジェクトのためのソースコード管理サービス

- Gitの仕組みを利用して、世界中の人々が自分の作品(プログラムコードやデザインデータなど)を保存、公開することができるようにしたウェブサービスの名称

- 複数人でプログラムを書く際に欠かせないサービス

---

# <font face="arial">GitHubは</font>
## <font face="arial">Gitホスティングサービスの一つ</font>

---

# <font face="arial">Gitホスティングサービスってなんぞ？</font>

---

## <font face="arial">Gitプロジェクトを置けるサービス</font>

---

## <font face="arial">じゃあGitプロジェクトって...</font>
##### <font face="arial">Gitによってバージョン管理されたプロジェクト(ファイル群)のこと</font>

---

## <font face="arial">有名なGitホスティングサービス</font>

<hr>

- GitHub(GitHub社)
![14%](https://anywher.net/wp-content/uploads/2014/11/logo-color_github.png)

- BitBucket(Atlassian社)
![60%](https://upload.wikimedia.org/wikipedia/commons/3/32/Atlassian_Bitbucket_Logo.png)

- GitLab(オープンソースソフトウェア)
![30%](https://about.gitlab.com/images/press/logo/wm_no_bg.svg)

---

## <font face="arial">Gitとは</font>
<hr>

- プログラムソースなどの変更履歴を管理する分散型のバージョン管理システムのこと。

詳しく説明してあるページ: http://www.backlog.jp/git-guide/intro/intro1_1.html

---

120525_ドキュメント_最新.txt
120602_ドキュメント.txt
120604_ドキュメント.txt
.
.
.
↑
バージョン管理されていないと、このようにバックアップされた過去のファイルが大量にできてしまう。

(しかも、どのファイルにどんなことが書いてあるか、一目で分からない)

---

`ドキュメント.txt`
![](/Users/AtsuyaSato/Desktop/Workshop/Assets/スクリーンショット%202017-01-26%202.24.59.png)

↑
バージョン管理されていると、変更点の差分が一目でわかるようになる。

---

## <font face="arial">GitHub Pagesとは</font>
<hr>

- GitHubが提供するホスティングサービスで、ウェブページをインターネット上に公開することができる。
- https://natmark.github.io/
↑
僕のポートフォリオサイトもGitHub Pagesで作成してます。

---

こんな感じで管理されてます。

![30%](/Users/AtsuyaSato/Desktop/Workshop/Assets/スクリーンショット%202017-01-21%2021.09.31.png)


![30%](/Users/AtsuyaSato/Desktop/Workshop/Assets/スクリーンショット%202017-01-21%2021.09.48.png)

---

### <font face="arial">説明するより、やってみた方が早いと思うので、さっそくGitHubのアカウントを作ってみましょう！</font>

---

ここからは同時に手順を説明します。


---

## <font face="arial">Gitが入っているか確認</font>

```
$ git --version
```

なければこちらからインストールできます。
http://git-scm.com/download

---


## <font face="arial">簡単なHTMLを書いてみよう</font>

index.html
```
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8" />
    <title>タイトル</title>
</head>
<body>
<h1>GitHub Pagesワークショップ</h1>
</body>
</html>
```

---

## <font face="arial">CSSを追加してみよう</font>

index.html
```
<head>
    <meta charset="UTF-8" />
    <link href="./style.css" rel="stylesheet" type="text/css">
    <title>タイトル</title>
</head>
```

style.css
```
h1{
	color: #f00;
}
```
---

