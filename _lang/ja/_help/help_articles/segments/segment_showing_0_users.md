---
nav_title: セグメント内のユーザーが見つかりません
article_title: セグメント内のユーザーが見つかりません
page_order: 1

page_type: solution
description: "このヘルプ記事では、セグメントに表示されているユーザー数がゼロでも、それ以上のユーザーが予想される場合のトラブルシューティング手順を説明します。"
tool: Segments
---

# セグメントにユーザーが存在しません

`0`ユーザーを確認する場合、考えられる解決策が 2 つありますが、予想していたのはそれだけではありません。
* [正確な統計の計算](#calculate-exact-statistics)
* [データ転送の検証](#verify-data-transfer)

## 正確な統計を計算

セグメント統計から推定値が得られる可能性があります。推定値は、結果の信頼区間が 95% のランダムサンプルに基づいて計算されます。`+/- 1%`ユーザーベースが小さいほど、セグメントのサイズが概算である可能性が高くなります。**セグメント詳細パネルの**「**正確な統計量の計算**」をクリックします。これにより、セグメント内の正確なユーザー数が計算されます。

![正確な統計量の計算オプションを表示するセグメント詳細パネル] [28]

## データ転送を確認

フィルタリングしているデータが Braze に送信されていない可能性があります。どのカスタムイベントが Braze に送信されているかを確認するには、[カスタムイベントレポートを参照してください][1]。

カスタムイベントと特定の日付とアプリを選択して、実際にどのデータがBrazeに転送されているかを確認してください。`0`データが Braze に送信されていることに気付いたら、次のステップは Braze へのイベントの送信方法を評価することです。

![カスタムイベント数がゼロと表示されるグラフ] [29]

{% alert important %}
Braze ダッシュボードに表示されるデータは、Braze に送信するデータと同じ構文ではない場合があります。これらの 2 つが完全に一致することを確認してください。
{% endalert %}

まだ助けが必要ですか？[サポートチケットを開きます]({{site.baseurl}}/braze_support/)。

_2021年1月5日に最終更新されました_

[1]: {{site.baseurl}}/user_guide/data_and_analytics/custom_data/custom_events/#custom-event-analytics
[28]: {% image_buster /assets/img_archive/trouble8.png %}
[29]: {% image_buster /assets/img_archive/trouble9.png %}
