
# Table of Contents

1.  [head](#org8831390)
2.  [license](#orgf2f6153)
3.  [課題](#orgdc4e16d)
4.  [課題](#org3ce1c3c)
5.  [aruba](#org7be9ec6)
6.  [Thor](#org0ee7fe0)
    1.  [gemひな形の作成](#org963f0b9)
7.  [jekyll](#org38448ba)
    1.  [概要](#org3e495bc)
    2.  [公式サイト](#org05af261)
    3.  [インストール](#org5b81395)
    4.  [使い方](#org904e186)
8.  [ゼミ](#orgf8d9187)
9.  [課題2](#orgaf5662c)
10. [RSpec](#org856e126)
    1.  [EXPECT(A).TO EQ B](#orgc1aec11)
    2.  [RSPEC &#x2013;INIT](#org12bb415)
11. [require\_relative](#orge515e8a)
12. [QUESTION<span class="timestamp-wrapper"><span class="timestamp">&lt;2019-06-24 月 12:33&gt;</span></span>](#org5a3ccf7)
    1.  [課題](#orgd5b3e3f)
13. [my\_help install<span class="timestamp-wrapper"><span class="timestamp">&lt;2019-06-17 月 13:49&gt;</span></span>](#org8f37d5f)
    1.  [data and time stamp(ここはasterisk二つ)](#org32f0753)
    2.  [show all](#org820eea0)
14. [read graduation thesis<span class="timestamp-wrapper"><span class="timestamp">&lt;2019-06-19 水 10:57&gt;</span></span>](#org5f51b64)
    1.  [Behaviour-Driven Development(BDD)](#org84812bc)
    2.  [Aim of BDD](#org8f4adab)
15. [read graduation thesis<span class="timestamp-wrapper"><span class="timestamp">&lt;2019-06-20 木 17:58&gt;</span></span>](#org7274b18)
    1.  [Cucumber and Rspec](#org10803bf)
16. [read graduation thesis<span class="timestamp-wrapper"><span class="timestamp">&lt;2019-06-21 金 18:47&gt;</span></span>](#orga9fd35b)
    1.  [Regexp](#orgd1e1082)
    2.  [hiki format](#org5774806)



<a id="org8831390"></a>

# head

-   blog


<a id="orgf2f6153"></a>

# license

-   cc by Shuhei Yamaguchi, 2019

\*blog


<a id="orgdc4e16d"></a>

# 課題

-   roman\_numeralのrspecを作る
-   下記のurlのfizzbuzをとりあえず写してみる(<https://qiita.com/tbpgr/items/41730edcdb07bb5b59ad>)
-   岡端が作成したmy\_helpのthorをテストしていく


<a id="org3ce1c3c"></a>

# 課題

-   arubaとcucumberの関係性を調べる,どのようにテストを書いていくかのサンプルを見せるmy\_helpのarubaによるテストの作成
-   jekyllでblog立ち上げる,githubとの連携


<a id="org7be9ec6"></a>

# aruba

spec.add\_development\_dependency "aruba"追加後のbundle installでffiに関してエラーが出た場合
Gemfileにgem 'ffi', '= 1.9.21'追加


<a id="org0ee7fe0"></a>

# Thor


<a id="org963f0b9"></a>

## gemひな形の作成

1.  bundle gem samplegem -b &#x2013;test
2.  ~.gemspecを編集
    spec.summary       = %q{Convert textile to markdown.}
    spec.description   = %q{Convert textile to markdown.}
    spec.homepage      = "<https://github.com/YumaInaura/textile2md>"
    に変更
3.  bundle install


<a id="org38448ba"></a>

# jekyll


<a id="org3e495bc"></a>

## 概要

-   静的サイトを作るためのジェネレーター
-   マークダウン記法


<a id="org05af261"></a>

## 公式サイト

jekyllrb.com


<a id="org5b81395"></a>

## インストール

gem bundle install


<a id="org904e186"></a>

## 使い方

-   作業ディレクトリ作成　mkdir~
-   フォルダ作成　jekyll new ~
-   HTMLファイル群作成 jekyll build 
    エラー出たら　bundle exec jekyll build
-   サーバー立ち上げ bundle serve
    エラー出たら　bundle exec jekyll serve


<a id="orgf8d9187"></a>

# ゼミ

bundle exec rake install local
git clone
rake
bundle update
bundle exec 


<a id="orgaf5662c"></a>

# 課題2

1.  jekyllのインストールの手順の問題点
2.  jekyllを動かせるようにする
3.  arubaの導入，書き方　<http://rikuga.me/2018/03/17/how-to-create-gem-using-thor/>
4.  src -> lib
5.  bundle gem test -b


<a id="org856e126"></a>

# RSpec

RSPEC.DESCRIBE クラス名DO
 IT "" DO
 END
END


<a id="orgc1aec11"></a>

## EXPECT(A).TO EQ B

AとBが等しいか比べる


<a id="org12bb415"></a>

## RSPEC &#x2013;INIT

CREATE   SPEC/SPEC\_HELPER.RB
CREATE   .RSPEC
参考<//QIITA.COM/LUCKYPOOL/ITEMS/E3662170033347510C3C>
    <//QS.NNDO.JP/UNIT-TEST-BY-RUBY-WITH-RSPEC>


<a id="orge515e8a"></a>

# require\_relative

実行したいファイルのディレクトリからの相対パスで書く


<a id="org5a3ccf7"></a>

# QUESTION<span class="timestamp-wrapper"><span class="timestamp">&lt;2019-06-24 月 12:33&gt;</span></span>

那須

1.  TDDのイメージが構造のテスト中心とありますが構造のテストとは
    -   テストとは二種類
        -   TDD 中身をわかっている　ホワイトボックス　コードの構造を考えていく　
        -   BDD 中身わからない　ブラックボックス　振る舞い
2.  HIKIとは
    -   hiki　wikiの一種
    -   wiki  cms(contents management system)の一種
    -   hiki記法　markuplanguage

3.RSPECとCUCUMBERの関係性　
　 - rspec rubyが用意しているテストの環境の一種 minitest utest(unittest)

-   cucumber BDDの環境 rspecの上に乗るようなsoftware

4.図6がRSPECで実行しているのにCUCUMBERの実行結果となっているのはなぜか
  そういう関係性だから
5.図7，図8がCUCUMBERで実行しているのにRSPECの実行結果となっているのはなぜか


<a id="orgd5b3e3f"></a>

## 課題

roman\_numeralsをrspecでテストする．


<a id="org8f37d5f"></a>

# my\_help install<span class="timestamp-wrapper"><span class="timestamp">&lt;2019-06-17 月 13:49&gt;</span></span>

my\_helpをinstallしました．

1.  my
2.  my\_help list
3.  my\_help new blog
4.  my\_help edit blog

であとは，orgの使い方


<a id="org32f0753"></a>

## data and time stamp(ここはasterisk二つ)

-   C-u C-c .
-   C-c . (date only +1 -2)


<a id="org820eea0"></a>

## show all

-   shift-tab


<a id="org5f51b64"></a>

# read graduation thesis<span class="timestamp-wrapper"><span class="timestamp">&lt;2019-06-19 水 10:57&gt;</span></span>

那須さんの卒業研究を読みました．


<a id="org84812bc"></a>

## Behaviour-Driven Development(BDD)

ビヘイビア駆動開発

1.  テスト駆動開発TDDの工程の理解を深めるものであり，説明するためのもの
2.  TDDのイメージは構造のテストを中心とするものであるのに対して，BDDはソフトの振る舞いを中心とする．


<a id="org8f4adab"></a>

## Aim of BDD

ソフトウェアが使われる状況を説明するための言語を単純化すること，ソフトウェア開発チームのコミュニケーションを後押しすること．


<a id="org7274b18"></a>

# read graduation thesis<span class="timestamp-wrapper"><span class="timestamp">&lt;2019-06-20 木 17:58&gt;</span></span>


<a id="org10803bf"></a>

## Cucumber and Rspec

1.Cucumberで一つのシナリオに焦点を当て,その振る舞いの主要点をかく.(一つずつ書いていく)

2.それぞれの主要点を実現するステップに分けて使用を決めていく．(TDDのred,green,refactoringの前に行う[使用を決める作業]に対応)

3.RSpecでテストコードを書き，red,green,refactoringを行う．

4.RSepecが成功すると，Cucumberのrefactoringを行う．


<a id="orga9fd35b"></a>

# read graduation thesis<span class="timestamp-wrapper"><span class="timestamp">&lt;2019-06-21 金 18:47&gt;</span></span>


<a id="orgd1e1082"></a>

## Regexp

正規表現


<a id="org5774806"></a>

## hiki format

<//GITHUB.COM/RUBIMA/RUBIMA/WIKI/HIKIFORMAT>

