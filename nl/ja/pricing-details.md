---

copyright:
  years: 2015, 2018, 2019
lastupdated: "2019-02-28"

subcollection: discovery

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:tip: .tip}
{:note: .note}
{:pre: .pre}
{:important: .important}
{:deprecated: .deprecated}
{:codeblock: .codeblock}
{:screen: .screen}
{:download: .download}
{:hide-dashboard: .hide-dashboard}
{:apikey: data-credential-placeholder='apikey'} 
{:url: data-credential-placeholder='url'}
{:curl: #curl .ph data-hd-programlang='curl'}
{:javascript: .ph data-hd-programlang='javascript'}
{:java: .ph data-hd-programlang='java'}
{:python: .ph data-hd-programlang='python'}
{:ruby: .ph data-hd-programlang='ruby'}
{:swift: .ph data-hd-programlang='swift'}
{:go: .ph data-hd-programlang='go'}

# Discovery の料金プラン
{: #discovery-pricing-plans}

{{site.data.keyword.discoveryfull}} サービスでは、お客様のニーズに合わせて異なるレベルのリソースと機能を選択できるように、**ライト**、**拡張**、および**プレミアム**の 3 つのプランが用意されています。
{: shortdesc}

**プライベート・データのユース・ケース**の機能、制限、および価格は次のとおりです。

## ライト
{: #lite}

サイズ | 文書ストレージ上限 | 文書数\* | 価格 
------ | ------ | ------ | ------  
N/A | 50 MB | 1,000/月 | 無料 

ライト・プランはスターター・プランであり、実動には使用しないでください。 有料プランにアップグレードする際、すべての取り込み済み文書を保持できます。  ライト・プランのインスタンスは、非アクティブ状態で 30 日経過すると削除されます。 

属性:
- 1 つの環境
- 最大 2 個のコレクション
- 無料の NLU エンリッチメント\*\*

追加オプションは、以下のとおりです。<br> [カスタム・モデル](/docs/services/discovery?topic=discovery-integrating-with-wks#integrating-your-custom-model):<br>
1 つの Watson Knowledge Studio モデルが含まれています。 追加モデル: 利用不可<br>[要素の分類](/docs/services/discovery?topic=discovery-element-classification#element-classification)\*\*\*:
1 カ月当たり 500 ページが含まれています。 追加ページ: 利用不可 <br>[ニュース照会](/docs/services/discovery?topic=discovery-watson-discovery-news#watson-discovery-news):
1 カ月当たり 200 件のニュース照会が含まれています。 追加の照会: 利用不可<br>[照会拡張](/docs/services/discovery?topic=discovery-query-concepts#query-expansion):
500 個の照会拡張と合計 1,000 個の用語。 追加の拡張: 利用不可

ライトから拡張へのアップグレードについては、[サービスのアップグレード](/docs/services/discovery?topic=discovery-upgrading-your-plan#service)を参照してください。

照会のパフォーマンスについては、[照会のパフォーマンス](/docs/services/discovery?topic=discovery-qp#qp)を参照してください。照会は、プランに基づいて制限されます。**ライト**・プランと**標準**プランの推定照会平均速度は、最上位テキスト・フィールドを 2 つ指定した、再ランク付けされた照会の場合、毎秒 1 照会です。

## 拡張
{: #advanced}

拡張プラン・サイズを選択する場合は、文書ストレージと照会の両方にリソースが必要になることに注意してください。そのため、プラン・サイズの文書上限に近づいており、以下の要件を満たす必要がある場合は、より大規模な環境が必要になる可能性があります。 

-  より高い照会パフォーマンス要件 (例えば、関連性トレーニングを使用している場合)
-  予想される同時ユーザー数が多い
-  複雑な照会の必要性 

照会のパフォーマンスに影響を与える要因について詳しくは、[照会のパフォーマンス](/docs/services/discovery?topic=discovery-qp#qp)を参照してください。照会は、プランに基づいて制限されます。**拡張** (S、MS) プランの推定照会平均速度は、最上位テキスト・フィールドを 2 つ指定した、再ランク付けされた照会の場合、毎秒 10 照会です。

サイズ | 文書ストレージ上限 | 文書数\* | 価格 
------ | ------ | ------ | ------ 
X スモール\*\*\*\* | 40 GB | 1 カ月当たり最大 50,000 文書 | 月額 $500 から  
スモール | 160 GB | 1 カ月当たり最大 1 M 文書 | 月額 $1,500 から  
ミディアム・スモール | 320 GB | 1 カ月当たり最大 2 M 文書 | 月額 $3,000 から 
ミディアム| 640 GB | 1 カ月当たり最大 4 M 文書 | 月額 $5,000 から 
ミディアム・ラージ | 1.2 TB | 1 カ月当たり最大 8 M 文書 | 月額 $10,000 から 
ラージ| 2.4 TB | 1 カ月当たり最大 16 M 文書 | 月額 $15,000 から 
X ラージ| 4 TB | 1 カ月当たり最大 32 M 文書 | 月額 $20,000 から 
XX ラージ | 5.5 TB | 1 カ月当たり最大 64 M 文書 | 月額 $35,000 から 
XXX ラージ | 12 TB | 1 カ月当たり最大 100 M 文書 | 月額 $45,000 から 

X スモールは使用可能な最小の環境であり、開発およびテスト専用環境として推奨しています。\*\*\*\*

拡張プラン内でレベルを変更する場合、新しいインスタンスを作成する必要はありません。 拡張プランからプレミアム・プランに切り替える場合は、新しいインスタンスが必要になります。 拡張プラン内でのティアのアップグレードについては、[拡張プラン内のティアの切り替え](/docs/services/discovery?topic=discovery-upgrading-your-plan#upgrading-your-plan)を参照してください。

\*\*\*\*X スモール・プランの特性: 
- 1 つの環境
- 最大 4 個のコレクション
- 無料の NLU エンリッチメント\*\*

その他すべての拡張プランの特性:
- 1 つの環境
- 最大 100 個のコレクション
- 無料の NLU エンリッチメント\*\*

追加オプションは、以下のとおりです。<br> [カスタム・モデル](/docs/services/discovery?topic=discovery-integrating-with-wks#integrating-your-custom-model):<br>
1 つの Watson Knowledge Studio モデルが含まれています。 追加モデル: 各 $800<br>[要素の分類](/docs/services/discovery?topic=discovery-element-classification#element-classification)\*\*\*:
1 カ月当たり 500 ページが含まれています。 追加ページ: 各 $0.40<br>[ニュース照会](/docs/services/discovery?topic=discovery-watson-discovery-news#watson-discovery-news):
1 カ月当たり 200 件のニュース照会が含まれています。  
10,000 件の追加照会 (1 カ月当たり): $0.10/照会<br>
10,001 から 100,000 件の追加照会 (1 カ月当たり): $0.05/照会<br>
100,000 件を超える照会 (1 カ月当たり): $0.03/照会<br>
[照会拡張](/docs/services/discovery?topic=discovery-query-concepts#query-expansion):
5,000 個の照会拡張と合計 25,000 個の用語。

`-----`
<br>
\* 文書上限は、ディスク上での平均 100 KB の文書サイズを想定しています。 文書サイズは、変換とエンリッチメントが行われた後に計算されます。このため、文書サイズは元の入力からは大幅に変わる可能性があります。 保管文書の数、および使用済みストレージの合計量は、[Environments](https://{DomainName}/apidocs/discovery#get-environment-info) API または [Collections](https://{DomainName}/apidocs/discovery#get-collection-details) API を使用するか、ツールを使用して表示できます。 文書がディスク上で平均 100 KB を超えている場合は、最大文書数制限に達する前にプランのストレージ上限に到達します。 文書に対して[文書セグメンテーション](/docs/services/discovery?topic=discovery-configservice#doc-segmentation)を実行すると、各セグメントが別個の文書としてカウントされます。

\*\* [自然言語理解 (NLU) エンリッチメント](/docs/services/discovery?topic=discovery-configservice#adding-enrichments)には、エンティティー抽出、センチメント分析、カテゴリー分類、概念のタグ付け、キーワード抽出、関係抽出、感情分析、要素の分類、および意味役割抽出があります。  各文書の最初の 50,000 文字のみがエンリッチされます。 

\*\*\*「要素の分類」は、管理文書全体を解析し、重要な要素を変換、識別、分類するエンリッチメントです。 これは、自然言語処理を使用して、PDF 文書からパーティー (対象者)、性質 (要素のタイプ)、およびカテゴリー (特定の種別) の各要素を抽出します。

新しい環境サイジング・オプション (`LT`、`XS`、`S`、`MS`、`M`、`ML`、`L`、`XL`、`XXL`、`XXXL`) を利用するには、API を使用して環境を作成するときに `2018-08-01` 以降の API バージョン日付を使用する必要があります。環境サイズの型は `string` になりました (以前のタイプは `integer` でした)。
{: note}

## プレミアム
{: #premiumplan}
   
プレミアム・プランは、より高い独立性とセキュリティーを提供するために、1 つ以上の Watson サービスの単一テナント・インスタンスを開発者および組織に提供します。 これらのプランでは、既存の共有プラットフォームにおける計算レベルの独立性が確保され、さらに転送中や静止中のエンドツーエンドの暗号化データが提供されます。 

プレミアム・プランの詳細情報またはプレミアム・プランのご購入については、[営業担当](https://ibm.biz/contact-wdc-premium)にお問い合わせください。 

## 追加情報
{: #pricingadd}

コストの計算については、[IBM Cloud 料金カリキュレーター ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://cloud.ibm.com/pricing/platform/watson){: new_window} を参照してください。

IBM Cloud セキュリティーについては、[Cloud Services data security and privacy![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://www.ibm.com/software/sla/sladb.nsf/sla/csdsp?OpenDocument){: new_window} を参照してください。

価格設定の追加情報については、[{{site.data.keyword.discoveryshort}} カタログ ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://cloud.ibm.com/catalog/services/discovery){: new_window} を参照してください。

## 既存のプランを使用中のお客様向けの注記
{: #pricingnotes}

- **2018 年 8 月 1 日**から、請求および使用量計算は、この価格設定プランに基づいて行われます。
- ライト・プランは、1 カ月当たり 2,000 文書/400 {{site.data.keyword.discoverynewsshort}} 照会から、1 カ月当たり 1,000 文書/200 {{site.data.keyword.discoverynewsshort}} 照会に削減されました。  新しいライト・プランの制限を既に超えている場合、これ以上文書を追加できません。 ただし、そのまま使用を継続するか、拡張プランまたはプレミアム・プランにアップグレードできます。
- 標準プランは廃止され、新規ユーザーがこのプランを使用することはできません。 既存の標準プランを現在使用している場合は、そのまま使用を継続するか、拡張プランまたはプレミアム・プランにアップグレードできます。
- 拡張プランとプレミアム・プランは、文書のティアに基づくようになり、文書の時間には基づかなくなりました。 毎月の請求は、ティアを切り替えない限り、文書数に基づいて変動することはありません。
- プレミアム・プランのお客様の場合、請求方法の変更について詳しくは、[営業担当![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://ibm.biz/contact-wdc-premium){: new_window}にお問い合わせください。	
