# gsc2019_Shogo-Hirasawa
 ３年 平澤彰悟です。2019年ゼミ論制作用レポジトリ

#### 課題目標　【機材管理システムの構築】  

 > 【達成項目】
   >> * UML方式のアクティビティ図を用いてフローチャート作成（2019/08/06）
   >> * ゼミ論のお題を変えたので0スタート【動画ファイル共有】→【機材管理システム構築】（2019/11/18）
   
 >【成果報告】
  >> * 2019/11/18　ゼミ論中間発表 https://docs.google.com/presentation/d/1IEv9esrZzojNQBrNbcIyaxE3yxBE_x60vZsmD_t0WzQ/edit?usp=sharing
  >> * 2019/12/05　ゼミ論中間発表 https://medium.com/furuhashilab/%E3%82%BC%E3%83%9F%E8%AB%96-%E6%A9%9F%E6%9D%90%E7%AE%A1%E7%90%86%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0-%E3%81%AE%E4%BD%9C%E6%88%90-fb317eea1c6

 >【ゼミ論提出用】
  >> https://docs.google.com/document/d/1-ZdNDABxnZ5sto2K3mBvoJPL5bwgtZVJQr-X1E92-JQ

>以下の内容がゼミ論である。文章はIMRAD形式に沿って展開していく

### Introduction
古橋研究室の機材として、iPad mini4 20台　MacBook Air 20台がある。これらの機材は先生のみならず学生にも利用できるものとなっている。しかし、管理体制が整っておらず効率的でかつ、安全な貸出ができていなかった。こういった状態を鑑みて、管理体制を整え、これら機材を誰もが使えるようにして、学生の生産性の向上を促すため、この研究を行った。現状の機材の管理体制は、先生一人で管理をおこなっているということになっている。なので、借りたい機材がある場合には先生に直接交渉して許可をもらわなければならない状態となっている。先生一人での管理では、記憶の限界もあるし、あれ程の機材を一人で管理するのは明らかにキャパシティをオーバーしている状態である。

### Methods
システムを構築するにあたり、Googleスプレッドシート（以下SS)とGoogleフォーム（以下フォーム）を使った。
Googleフォームで貸し出しと返却の際に利用者に情報を入力してもらう。その入力した情報をSS上で管理する。管理している情報をSSでガントチャート方式で表示し、誰が何をいつまで借りるのかということを表示する。フォームは貸出用と返却用で同じ内容の質問項目となっている。
フォームURL 貸出用 https://docs.google.com/forms/d/10FrDeVom4cKn0-u4i6e6D7KPWpC3kBC1WaCNNg8rJNg/edit?usp=sharing
          返却用 https://docs.google.com/forms/d/19mYLTsYTVuYX5tLZCmOI7NW2bECPoIDNXMZWVcPd_UY/edit?usp=sharing
質問内容は氏名・学籍番号・借りるor返すものとなっている。そこからSSにデータを自動送信させる。そのデータを別シートである、ガントチャートに反映させる。ガントチャートはSSのアドオン(Projectsheet Planning)を使用した。

借りる際に学生自身責任感を持ってもらうためのルール作りも行った。
機材の未返却、故意による破損、盗難があった場合、追加課題のペナルティまたは、ゼミの単位剥奪というルール作りを行った。借りる上の担保の役割でこのルールが役に立つと推測される。具体的なペナルティは、国際会議または防災訓練の追加参加。グラレコやマッピングの追加課題を想定している。

### Results
機材管理システムを構築することにより、誰でも機材を借りられ、作業が効率的になることがわかった。また、当研究室ではApple製品を使っている学生が多く、研究をする上でApple製品を持っていない学生からの需要が高いことがわかった。タブレットやPCのみならず、研究室には様々な備品があることが判明した。また、それら他の部品に対しても需要があることがわかった。特にドローンの貸出需要があることが判明した。貸し出す種類や個数が増えていくにつれ、フォームの編集が必要であると思う。また、改めて、研究室の備品の何に対し需要があるのか、それは貸出可能なのかということを調べる必要を感じた。

### Discussion
機材の管理という問題は、当研究室のみならず部活やサークル、会社などで起こる珍しくない問題であると感じた。機材を管理する上で紙媒体で管理する方法もある。しかし紙媒体では紛失の危険性がある。それ故にインターネット上で管理する意味があると考えた。また、比較的機能性が高く、普及性も高いSSとフォームを使うことにより、無料で使え、かつウェブまたはプログラミング知識がなくても運営しやすいものとなっている。
無料でかつ手軽なものとなっているので、学生組織や会社などの団体でも誰でも気軽に導入しやすいシステムとなっている。

### Conclusion
今回の研究だけでは、機材管理システムとしてまだ盤石とは言えないと感じた。未完であるこのシステムをより確実なものにするためには以下の問題点を解決する必要があると考える。

1.減価償却の判断の仕方
2.機材の初期化へのルール
3.定期的な機材のメンテナンスを誰がするのか
4.故障した時の対応

1.減価償却の判断の仕方
iPad、MacBook共に消耗品であるため、使えば使うほどパフォーマンスが落ちてくる。定期的に診断し、パフォーマンスの低下を見極める必要があると考える。また減価償却を一つの機材に偏らせないために、棚を作り、棚の左から借りて返却時には右から返すなどの工夫が必要であると考える。

2.機材の初期化へのルール
iPad、MacBook内に入っているデータや設定は使う度に初期化しないと、次使う人に迷惑がかかる。そのため利用者には毎回返却する前に初期化してもらわなければならない。そのためのルール作りが必要になる。

3.定期的な機材のメンテナンスを誰がするのか
定期的なメンテナンスを行わないと、故障したままの機材が貸し出される可能性が出てくる。また、どのタイミングで壊れたのかということがわからなくなり、責任問題があやふやになる恐れがある。メンテナンスは必要であり、この作業を誰が担うのかというのとが、問題であると考える。

4.故障した時の対応
故意でなくても、故障する場合は考えられる。また、機材の寿命で故障することもある。そういったときに、誰が修理をして資金はどこから降りるのかを明確にする必要があると感じた。

### Reference

### Acknowledgements
本研究を進めるにあたり青山学院大学地球社会共生学部 教授の古橋大地氏をはじめ多くの方々より多大な助言を賜りました。厚く感謝を申し上げます。


