omnioutliner-opml2html
======================

convert OPML from OmniOutliner to HTML

## 説明

Mac OS XのアウトラインプロセッサOmniOutlinerで保存したOPMLをHTMLに変換するもの。汎用性はない。[opml2html.pl](http://jerermy.zawodny.com/blog/)をいじった。

OmniOutliner には以下のようなHTML出力方法がすでにいくつかあるが、どれも希望にあわなかったため作成:

* OmniOutlinerネイティブのHTML出力
  * ノート部分が改行なしにベタで出てしまう。意味ない<div>とフォントスタイル指定ばかりで、htmlとして(再)利用性が話にならない
* [OmniOutliner: Extras](http://www.omnigroup.com/applications/omnioutliner/extras/)にある AppleScript
  * 動かすとOmniOutlinerごと落ちる。たまに成功しても滅茶苦茶なHTMLが出る。
* 同じく[OmniOutliner: Extras](http://www.omnigroup.com/applications/omnioutliner/extras/)
にある Export from OmniOutliner to Microsoft Word
  * 動かない。

## 動作環境

    use XML::Simple;
    use Data::Dumper;
    use HTML::Entities;

って感じなので、必要なものをCPANなりapt-getなりperl -MCPAN -e shellしてインストール

## 使い方

    omnioutliner-opml2html &lt; sample.opml &gt; sample.html

## Copyright

opml2html.plに従う.

    # opml2html.pl, (c) Jeremy Zawodny -- http://jerermy.zawodny.com/blog/
    #
    #   Updated by Michael Radwin (http://www.radwin.org/michael/blog/)
    #   on Dec 26th, 2003 to include image size attributes and link
    #   titles.
    #
    # You may distribute this code freely.  It's not rocket science.
