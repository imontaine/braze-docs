---
nav_title: アクセシブルなメッセージングを構築する
article_title: Brazeでアクセシブルなメッセージを作る
page_order: 3.5
page_type: reference
description: "この参考記事では、マーケティングコンテンツでアクセシビリティを考慮することが重要な理由と、Brazeでアクセシブルなメッセージを作成する方法について説明する。"
---

# Brazeでアクセシブルなメッセージを作る

> たとえ意図的でなくとも、障害者を排除したマーケター・コンテンツは、何百万人もの人々があなたのブランドと交流することを妨げる可能性がある。マーケティングにおけるアクセシビリティとは、誰もが簡単にマーケティングを体験し、コミュニケーションを受け、理解し、製品やサービス、ブランドに投資したりファンになったりできるようにすることである。メッセージングをデザインする際には、どのようにすればすべての顧客がデザインにアクセスできるようになるかを検討するために、特別な時間をかけること。

## なぜアクセシビリティが重要なのか

- **ユーザビリティが向上した：**アクセシビリティは、ユーザーがコンテンツとどのようにインタラクションするかを考えているため、アプリやサイトのユーザビリティについて考えることを促す。つまり、アクセシビリティは多くの場合、障害を持つユーザーだけでなく、すべてのユーザーのオンライン体験を向上させるのだ。
- **マーケターへのリーチを広げる：**障害者の世界市場は10億人を超え、その消費力は7兆ドル近くに達する。
   > 「障がい者のマーケットは大きく、世界人口の高齢化とともに成長している。大きな障害者マーケターがパープル・ポンドと呼ばれる英国では、障害者とその家族は毎年少なくとも2490億ポンドを費やしている。米国では、障害者の年間裁量支出は2000億ドルを超えている。世界の障害者市場は7兆ドル近いと推定されている」。<br>*ソース[W3C](https://www.w3.org/WAI/business-case/)*
- **法的リスクを最小限に抑える：**多くの国で、デジタル・アクセシビリティを義務付ける法律がある。

## 考慮すべき障害分野

*このセクションは、[W3Cから一部引用している：多様な能力と障壁](https://www.w3.org/WAI/people-use-web/abilities-barriers/).*

### ビジュアル

視覚障害には、片目または両眼の軽度または中等度の視力喪失から、両眼の視力の大幅な喪失または完全な喪失まで、さまざまなものがある。人によっては、特定の色に対する感受性が低下したり欠如したり、明るい色に対する感受性が亢進したりする。

あなたのコンテンツとインタラクトするために、これらのユーザーは以下の能力を必要としている：

- 文字や画像を拡大・縮小する
- フォント、色、スペーシングの設定をカスタマイズする
- コンテンツの音声合成を聞く（つまり、スクリーンリーダーを使う）
- 動画の音声解説を聞く
- リフレッシュ点字を使って文字を読む

{% alert note %}
- 世界では、少なくとも22億人が近視または遠視の障害を持っている（[WHO](https://www.who.int/news-room/fact-sheets/detail/blindness-and-visual-impairment)参照）。
- 男性の約12人に1人、女性の約200人に1人がある程度の色覚異常があり、世界には推定3億人がいる（[NHS](https://www.nhs.uk/conditions/colour-vision-deficiency/)参照）。
{% endalert %}

### ヒアリング

聴覚障害には、片耳または両耳の軽度から中等度の聴覚障害が含まれる。部分的な難聴であっても、オーディオ・コンテンツに関しては問題になることがある。

あなたのコンテンツを理解するために、これらのユーザーは頼りにしている：

- 音声コンテンツのトランスクリプトとキャプション
- キャプションを表示し、キャプションの文字サイズや色を調整するオプションを提供するメディアプレーヤー
- オーディオコンテンツの停止、一時停止、音量調整のオプション（システム音量とは独立系）
- バックグラウンドノイズと明瞭に区別できる高品質なフォアグラウンドオーディオ

{% alert note %}
- 標準的な聴力検査によると、米国では12歳以上の8人に1人（13％、3000万人）が両耳に難聴がある。
- 18歳以上の米国成人の約15％（3750万人）が、何らかの聴覚障害をレポートしている（[NIH](https://www.nidcd.nih.gov/health/statistics/quick-statistics-hearing)参照）。
{% endalert %}

### フィジカル

身体障害には、筋力低下や筋肉のコントロールや感覚の制限、関節障害、運動を妨げる痛み、手足の欠損などがある。

このようなユーザーは、（標準的なキーボードを使用していなくても）機能を有効にするためにキーボードのサポートに依存している。あなたのコンテンツと対話するために、これらのユーザーは必要とする：

- 大きなクリック可能エリア
- タスクを完了するのに十分な時間
- Currentsの目に見える指標
- ページヘッダーやナビゲーションバーのようなコンテンツブロックをスキップするメカニズム

{% alert note %}
米国では200万人近くが手足を失った状態で生活している（[切断者連合](https://www.amputee-coalition.org/limb-loss-resource-center/resources-filtered/resources-by-topic/limb-loss-statistics/limb-loss-statistics/#1)参照）。
{% endalert %}

### 認知的

認知障害、学習障害、神経学的障害には、神経多様性や神経学的障害のほか、必ずしも神経学的ではない行動障害や精神衛生上の障害も含まれる。神経系のあらゆる部分に影響を及ぼし、聴覚、運動、視覚、会話、情報の理解などに影響を及ぼす。

個々のニーズに応じて、これらのユーザーは以下を頼りにしている：

- 明確に構成されたコンテンツ
- フォーム、ボタン、その他のコンテンツに一貫したラベルを付ける
- 予測可能なリンクターゲットと全体的な相互作用
- メニューや検索バーなど、さまざまなナビゲーション方法
- 点滅、点滅、またはその他の邪魔なコンテンツをオフにする設定
- 画像, 写真に支えられたシンプルなテキスト


{% alert note %}
- 米国では5人に1人が学習や注意の問題を抱えている（[LDA](https://ldaamerica.org/lda_today/the-state-of-learning-disabilities-today/#:~:text=LD%20Today,have%20learning%20and%20attention%20issues.)参照）。
- 世界人口のおよそ10～20％がニューロダイバージェントと考えられている（[デロイトを](https://www2.deloitte.com/us/en/insights/topics/talent/neurodiversity-in-the-workplace.html)参照）。
- 世界で約100人に1人が自閉症である（[WHO](https://www.who.int/news-room/fact-sheets/detail/autism-spectrum-disorders)参照）。
{% endalert %}

## ベストプラクティス

### コンテンツ

- コンテンツはブランドを保ちつつ、平易な言葉を使う。米国中学1年生レベルの読解力で書く。[ヘミングウェイ・アプリなどの](https://hemingwayapp.com/)リソースを使って、テキストの読解レベルをチェックすることができる。
- コンテンツを論理的に構成し、見出しが正しい階層に従っていることを確認する。見出しのレベルを飛ばしてはいけない。
- 長いコンテンツの塊には、中央揃えテキストを避ける。これは、認知障害や学習障害のあるユーザーには読みにくいかもしれない。2行以上に折り返すコンテンツは左寄せにする。
- デジタル機器で読みやすいサンセリフフォントを使用する。
- テキストが切り捨てられていないことを確認するために、デバイスに[テストメッセージを送信]({{site.baseurl}}/user_guide/engagement_tools/campaigns/testing_and_more/sending_test_push_notifications/)してコピーを常にテストすること。もしあなたのメッセージが途切れてしまうと、あなたのコンテンツがユーザーに届かなくなるため、あなたにとってもユーザーにとっても痛手となる。

### リンク

ナビゲーションのためにリンクを使い、ユーザーを外部ページに誘導する。

{% alert tip %}
ボタンのように見え、ボタンのように動作するものが欲しければ、リンクをボタンのようにスタイリングするのではなく、常に実際のボタンを使うようにしよう。リンクとボタンは、一般ユーザーにとっては同じように感じられるかもしれない-マウスを使ってリンクやボタンにカーソルを合わせ、マウスでクリックすることができる-しかし、ボタンとリンクはコントロールが異なる（例えば、ボタンは<kbd>スペース</kbd>キーや<kbd>Enter</kbd>キーを押すことでアクティブにできるが、リンクは<kbd>Enter</kbd>キーでしかアクティブにできない）ため、リンクをボタンのようにスタイルすると混乱する可能性がある。
{% endalert %}

リンクがユーザーをどこに連れて行くかを明確に説明するリンクテキストを書く。スクリーンリーダーのユーザーは、コンテンツに目を通す手段として、リンクからリンクへとスキップすることが多い。ここをクリック」「もっと見る」「詳細はクリック」といったフレーズは、文脈を無視して読むと曖昧になるので避けること。

たとえば、天気レポートを見るためのリンクをどう書くかを考えてみよう。

| 悪い  | より良い | ベスト |
| --- | --- | --- | 
| ここをクリック | 今日の天気にアクセスするにはここをクリック | 今日の天気 |
{: .reset-td-br-1 .reset-td-br-2 .reset-td-br-3}

すべてのコンテンツに言えることだが、できるだけ余計な言葉を使わず、端的に書くこと。

### ボタン

フォームの送信やカルーセルの再生など、クリック可能なアクションにはボタンを使う。

リンクテキストと同様に、ユーザーがボタンを押したときに起こるアクションを明確に説明するボタンテキストを書く（例えば、「続きを読む」ではなく「全文を読む」）。ボタンのテキストが長すぎないかテストする。ボタンがすべてのテキストを表示できない場合は、テキストが改行されるのではなく、省略記号で切り捨てられる。

### 画像、写真

マーケティング・コンテンツの画像写真を見ることができないユーザーもいる。アクセシビリティを考慮しないと、画像写真が、すべてのユーザーが同じコンテンツを受け取る際の障壁になりかねない。

#### オルトテキスト

代替テキストとは、スクリーンリーダーやその他の支援技術がユーザーに提供する、画像の内容に関する短い説明である。

- すべての画像写真について、その画像の情報や機能を提供する代替テキストを書く。
- 画像, 写真が[装飾的な](https://www.w3.org/WAI/tutorials/images/decorative/)場合（コンテンツに追加しない）、空のアトリビューション（`alt=""` ）を使用する。
- altテキストに "画像 "や "写真 "という言葉を使わないこと。

#### 画像、写真

スクリーン・リーダーは画像、写真に含まれるテキストを読むことができないので、テキストの画像は使わないこと。また、テキストの画像もうまくリサイズできず、ユーザーのニーズや好みに合わせてカスタマイズすることもできない。実際のテキストでは、ユーザーは色やコントラストなどをカスタマイズでき、品質を落とすことなくテキストのサイズを変更できる。文字の画像, 写真が拡大されると、ピクセル化され、品質が低下し、読みにくくなる。

### ビデオ

動画にクローズドキャプションを提供する。視力が低下している人、騒がしい場所で視聴している人、動画の言語とは異なる言語を話す人の助けになる。

### カラーコントラスト

十分な色のコントラストを持たせることは、アクセシビリティを向上させる手っ取り早い方法だ。前景色（テキスト）とバックグラウンドの色のコントラスト比は、[WCAG2.1のAAレベル要件に](https://www.w3.org/TR/WCAG/#contrast-minimum)準拠すべきである：

- 通常のテキスト（本文、ボタン、リンクなど）のコントラスト比は4.5:1。
- 大きなテキスト（ヘッダーを考える）のコントラスト比は3：1である。

[WebAimのコントラストチェッカーツールを](https://webaim.org/resources/contrastchecker/)使えば、背景色に対してテキストが読めるかどうかを確認できる。

### フォーム

**長いフォームを細かく切り分ける**<br>認知的な読み込みを減らすために、長いフォームを小さなセクションに分割する。これはチャンキングと呼ばれ、情報を消費しやすくするために使われる段階的な情報開示パターンである。これはすべてのユーザーにとって有益だが、特に認知障害を持つ人々にとって有用である。

**ツールチップやその他のホバー・ステートで重要なコンテンツを隠さない**<br>ホバー状態に含まれるコンテンツは、発見しにくく、モバイルフレンドリーではない。また、画面拡大機能を使っているユーザーは、ホバーでしか利用できないコンテンツを見るのに苦労するだろう。

**フィールド内の無効な文字のブロックを避ける**<br>フォームフィールドに特定の文字種が入力できないようにしない。ユーザーが好きなように入力できるようにし、何が間違っているのかエラーメッセージを出す方がいい。キーボード入力をブロックすることは、支援技術ユーザーにとって特に問題となる。なぜなら、彼らはフォームに正しく入力されたかどうかを判断するために、インライン・バリデーションに大きく依存しているからだ。

**明確なエラーメッセージを書く**<br>良いエラーメッセージは3つの部分で構成されている：何が起こったのか、何が間違っていたのか、どうすれば修正できるのか。エラーメッセージは明確で理解しやすいものでなければならない。簡単な言葉で話すようにする。専門用語は必要ない。
<br>

### カスタムHTML

メッセージングにカスタムHTMLを使用している場合：

- [セマンティックHTMLを](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML)使う。これは、ある要素を別の要素のように見せるためにスタイルを設定するのではなく、本来の目的に合った正しいHTML要素を使用することを意味する。ほとんどのHTML要素には、独自のアクセシビリティ・サポートが組み込まれている。
- コンテンツの言語を識別するために、HTML内に言語属性を設定する。スクリーン・リーダーは、各言語の発音や特徴に基づいて、言語ごとに異なるサウンド・ライブラリを使用する。言語が指定されていれば、スクリーン・リーダーは必要に応じて自動的に言語ライブラリを切り替えることができる。以下に例を示します。

{% raw %}
```html
<html lang="en-us">
```
{% endraw %}

