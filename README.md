omnioutliner-opml2html
======================

convert OPML from OmniOutliner to HTML

## ����

Mac OS X�Υ����ȥ饤��ץ��å�OmniOutliner����¸����OPML��HTML���Ѵ������Ρ��������Ϥʤ���[opml2html.pl](http://jerermy.zawodny.com/blog/)�򤤤��ä���

OmniOutliner �ˤϰʲ��Τ褦��HTML������ˡ�����Ǥˤ����Ĥ����뤬���ɤ���˾�ˤ���ʤ��ä��������:

* OmniOutliner�ͥ��ƥ��֤�HTML����
  * �Ρ�����ʬ�����Ԥʤ��˥٥��ǽФƤ��ޤ�����̣�ʤ�<div>�ȥե���ȥ����������Ф���ǡ�html�Ȥ���(��)���������äˤʤ�ʤ�
* [OmniOutliner: Extras](http://www.omnigroup.com/applications/omnioutliner/extras/)�ˤ��� AppleScript
  * ư������OmniOutliner��������롣���ޤ��������Ƥ���������HTML���Ф롣
* Ʊ����[OmniOutliner: Extras](http://www.omnigroup.com/applications/omnioutliner/extras/)
�ˤ��� Export from OmniOutliner to Microsoft Word
  * ư���ʤ���

## ư��Ķ�

    use XML::Simple;
    use Data::Dumper;
    use HTML::Entities;

�äƴ����ʤΤǡ�ɬ�פʤ�Τ�CPAN�ʤ�apt-get�ʤ�perl -MCPAN -e shell���ƥ��󥹥ȡ���

## �Ȥ���

    omnioutliner-opml2html &lt; sample.opml &gt; sample.html

## Copyright

opml2html.pl�˽���.

    # opml2html.pl, (c) Jeremy Zawodny -- http://jerermy.zawodny.com/blog/
    #
    #   Updated by Michael Radwin (http://www.radwin.org/michael/blog/)
    #   on Dec 26th, 2003 to include image size attributes and link
    #   titles.
    #
    # You may distribute this code freely.  It's not rocket science.
