# OpenCV LiDAR C++ 시작해보기
<div style="text-align: right">건국대학교 일반대학원 전기기계 및 전력전자 노태형</div><br>

## 서론
일본에서 학부졸업 전 중고시장에서 어렵게구한 LiDAR였지만 연구실에 들어와 이리치이고 저리치이는 사이 한구석에서 썪고 있었습니다.
요번 ROS 국비교육을 통해 Robot에 대해 굉장히 관심있는 여러분들과 함꼐 다시 처음부터 시작하며 알아보고 기록하는 시간을 가지고자 합니다.

목차
- 서론
- 1. 리얼센스 개요
- 2. LiDAR를 사용하기에 앞서 환경구축해야할 것들
- 3. 図に変換してみましょう。
- 4. もっと修正を加えてみましょう。
- 5. 実際の活用例
- おわりに
## i. 리얼센스 개요
Overview
인텔 리얼센스 SDK 2.0은 뎁스 카메라 (D400 & L500와 SR300) 크로스 플랫폼 라이브러리이다.

SDK는 깊이와 칼라 스트리밍, 내부와 외부의 교정 정보를 제공해준다.(intrinsic and extrinsic calibration information)

라이브러리는 통합적인 스트림들(pointcloud, depth and color streaming과 vise-versa)
과 스트리밍 세션의 record와 playback(코드 있음) 빌트인 서포트를 제공한다.


![mandara](./images/mandara.png#center)<br>
**図1．曼荼羅図**
## ii. 優先度をつけましょう！
やることリストの作成が終わったとしたら書いたやることリストに対して優先度を付けます。
優先度は高、中、低の順位で先にやらないと次のやることリストに行けないことを高い優先度を付けることで
全体的に優先しないといけないことを分かることができます。
これを図に起こしたものが次に紹介する**WBS(Work Breakdown Structure）**
のことです。
## iii. 図に変換してみましょう。
![prototype](./images/prototype.png)<br>
**図2．WBS及びガントチャート**<br>
この図は私が就職する予定の会社から例題としてもらったものです。
区分１から５まで基準点の例としては
|区分|期間|説明|
|------|---|---|
|１|6か月|半年で終わる計画|
|２|3が月|3か月で終わる計画|
|３|1か月|1か月ことで分かれるもの|
|４|2週|2週以内で終わる仕事|
|５|1週|一番細かく分けた項目|

となります。これはあくまで例であるためもっと個人やチーム計画に合わせるように
期間とかを修正した方がいいと思います。
--ガントチャートの説明--
## iv. もっと修正を加えてみましょう。
あくまで先の物は貰ったものであるためもっと今回、私のプロジェクトに適用するためには工夫が必要になりました。
先ず、12名のチームであるためそれぞれのやることリストに担当者欄が必要でした。
また、仕事を用意したけど納期を守らない、守らない理由にはそれを監督したり管理してくれる責任者がいないことに気が付きました。
それと先生と相談した結果、責任者が確認したことを署名するための責任者印と必ず成果物を確認しないと私たちは実物を作らないといけないため成果物を確認しないといけないことでした。
まとめると下の図3のように項目を追加しました。<br>
![custom](./images/custom.png)<br>
**図3．改善したWBS及びガントチャート**<br>
それと一つの画面に収まるため右にあるメモを外しました。12人のチームになるとやることリストが増えすぎて結局右のメモが見ずらかったためです。

## v．実際の活用例
![example](./images/example.png)<br>
**図4. 実際の使用したWBS及びガントチャート**<br>
私たちは今回、作品作りで設計、開発に分けて色を付けて区分を行いました。
期間を書いてその通り図4に見えるようにガントチャートを構成し延長したら延長した分を黄色で塗りつぶし
すぐ見つかるようにしました。計画は早かった時には＊表示を計画が全然ガントチャート通りに行かなかった場合はXを表示し
なるべくその当時の進捗度を把握し遅かったり早かったりし時、フィードバックを受けながら、それとも出しながら今回の作品を
作り上げました。

## おわりに
今回は学校の卒業作品展に向けて開発者ではなくプロジェクトリーダーとして勤めました。チームリーダーとかは今まで何回やったことがありましたが10人以上のチームのリーダーになったのは今回は初めてですね。
紆余曲折を重なって4年間一緒に過ごした仲間たちだったとしても流石に余裕を持って上手くは行かなかったんでした。だがこんな経験少ないプロジェットリーダーとしても話を聞いて作品を作り上げった私の自慢な
仲間たちがあってこそ今回の作品が出来上がったと思います。今回のプロジェクトマネジメントが最高の結果だとは思いませんが最善を尽くしたものだと考えております。皆さんには個人の個性が反映された最善の
プロジェクトマネジメントが出来上がるため私の今回の記事が役に立つように願っております。

github Address:https://github.com/Madness-Ro/project-miraisouzouten-document
![example](./images/QR-code.png)
Special Thanks<br>
HAL東京先端ロボット開発学科　担当　山口　直彦先生<br>
韓国　SUNGAM電気　R＆D部署　担当　Choi Jae-Hyuk<br>
先端ロボット開発学科の仲間たち

未来創造展2022　
https://miraisozoten.com TH452


