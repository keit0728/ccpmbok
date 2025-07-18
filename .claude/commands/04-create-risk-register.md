# リスク登録簿作成

プロジェクトのリスク登録簿を作成・管理します。

## 説明

プロジェクトのリスクを体系的に識別、分析、対応計画を策定し、継続的に管理するためのリスク登録簿を作成します。リスクの定量的・定性的分析を行い、優先順位付けと対応策を記録します。

## 手順

1. 初期設定：

   - プロジェクト名
   - リスクレビューの頻度（週次/隔週）

2. リスク分析基準の確認・調整：

   - 発生確率の定義（5 段階）
   - 影響度の定義（コスト、スケジュール、品質の観点）
   - リスクスコアの算出方法（確率 × 影響度）
   - 対応が必要なスコアの閾値

3. リスクの識別（ブレーンストーミング形式で実施）：

   **カテゴリ別にリスクを確認**

   - 技術リスク：「技術的な実現可能性や複雑性に関するリスクはありますか？」
   - スケジュールリスク：「納期やマイルストーンに影響するリスクは？」
   - コストリスク：「予算超過の可能性があるリスクは？」
   - 品質リスク：「品質基準を満たせないリスクは？」
   - リソースリスク：「要員やスキルに関するリスクは？」
   - 外部リスク：「法規制、市場、天災などの外部要因は？」

4. 各リスクの詳細情報を収集：

   - リスク ID（自動採番：R001, R002...）
   - リスク名（簡潔な名称）
   - 詳細説明（「もし〜ならば、〜になる」形式）
   - 根本原因
   - 発生確率（1-5）
   - 影響度（1-5）
   - リスクスコア（自動計算）
   - リスクの兆候（トリガー）

5. リスク対応戦略の策定：

   - スコアに基づく対応戦略の選択
     - 20-25：緊急対応（回避または軽減必須）
     - 15-19：優先対応（軽減推奨）
     - 10-14：要対応（軽減または受容）
     - 5-9：監視（受容し監視）
     - 1-4：受容可（特別な対応不要）
   - 具体的な対応策
   - 責任者の割当
   - 対応期限

6. 定量的分析（重要リスクのみ）：

   - 予想損失額
   - 対策コスト
   - 期待金銭価値（EMV）

7. リスク対応計画の詳細化：

   - 予防的対策（リスク発生前）
   - 発生時対策（コンティンジェンシープラン）
   - 二次リスクの識別
   - 残存リスクの評価

8. 継続的な管理プロセス：

   - 新規リスクの追加
   - 既存リスクの再評価
   - 対応策の進捗確認
   - 顕在化したリスクの課題への転換

9. ドキュメントを`docs/04_risk_register.md`として保存します。

## 対話的な作成プロセス

1. 「プロジェクトで最も心配していることは何ですか？」から開始
2. 各カテゴリについて体系的に確認
3. 「このリスクが発生する確率はどの程度ですか？」で定量化
4. 「発生した場合の影響はどの程度ですか？」で影響度評価
5. 「どのような対策が考えられますか？」で対応策検討

## 注意事項

- **リスクと課題の区別**: すでに発生している事象は「課題」として別管理
- **定期的な更新**: 週次でのレビューと更新が成功の鍵
- **ポジティブリスク**: 機会（好影響）も記録することを検討
- **正直な評価**: リスクを隠さず、正直に評価・共有

## 更新時のチェックポイント

- [ ] 新しいリスクは発生していないか？
- [ ] 既存リスクの確率や影響度は変化していないか？
- [ ] 対応策は効果的に機能しているか？
- [ ] クローズできるリスクはないか？
- [ ] 顕在化したリスクはないか？

## 使用するテンプレート

`template/04_risk_register.md` をベースに作成し、プロジェクトの進行に応じて継続的に更新します。
