# 新規学習分野セットアップ指示書

## 概要

新しい学習分野を追加する際に、AIエージェントが学習者と対話して適切な学習範囲・目標を設定し、必要なメタデータファイルを生成するための指示書。

## AIエージェントの役割

学習者との対話を通じて以下を実行する：

1. **学習分野の絞り込み**
2. **現在の知識レベルの把握**
3. **学習目標の明確化**
4. **適切なメタデータファイルの生成**
5. **初期学習コンテンツの構造化**

## 対話プロセス

### ステップ1: 基本情報の収集

以下の質問を通じて学習分野を絞り込む：

**Q1: 学習分野名**
- 「何について学びたいですか？」

**Q2: 現在の知識レベル**
- 「この分野について、現在どの程度ご存知ですか？」
- 「すでに理解している概念やキーワードがあれば教えてください」
- 「過去に学習経験はありますか？」

**Q3: 学習目的・動機**
- 「なぜこの分野を学びたいのですか？」
- 「学習後にどのようなことができるようになりたいですか？」

### ステップ2: 範囲の絞り込み

**Q4: 興味のある側面**
- 「この分野の中で、特に興味のある側面はありますか？」
- 「理論的な理解と実践的な応用、どちらに重点を置きたいですか？」

**Q5: 学習レベル**
- 「どのレベルまで学習したいですか？（基礎、中級、応用）」
- 「最終的に人に説明できるレベルを目指しますか？」

### ステップ3: 具体的な目標設定

**Q6: 成功指標**
- 「学習が完了したと判断する基準は何ですか？」
- 「具体的にできるようになりたいことはありますか？」

**Q7: 学習方法の希望**
- 「どのような学習方法が好みですか？（読解中心、実践中心、対話中心など）」
- 「避けたい学習方法はありますか？」

## 生成すべきファイル

対話結果を基に以下のファイルを `/subjects/{学習分野名}/` に生成する：

### 1. metadata.md
```markdown
# {学習分野名} - メタデータ

## 基本情報
- **学習分野**: {分野名}
- **作成日**: {日付}
- **学習者の背景**: {現在の知識レベル}

## 学習目的
{学習動機・目的}

## 学習範囲
{絞り込んだ具体的な範囲}

## 最終目標
{具体的な成功指標}

## 学習方法の希望
{希望する学習スタイル}
```

### 2. scope-definition.md
```markdown
# 学習範囲定義

## 含まれる内容
- {学習に含める概念・トピック}

## 除外する内容
- {明示的に除外する範囲}

## 重点領域
- {特に重点を置く領域}

## 前提知識
- {学習者が既に持っている知識}
```

### 3. knowledge-baseline.md
```markdown
# 現在の知識レベル

## 既知の概念
- {学習者が既に理解している概念}

## 不明確な概念
- {曖昧な理解の概念}

## 未知の概念
- {全く知らない概念}

## 経験・実践
- {関連する実践経験}
```

### 4. learning-objectives.md
```markdown
# 学習目標

## 最終目標
{最終的な到達目標}

## 段階的目標
### 基礎段階
- {基礎レベルの具体的目標}

### 中級段階
- {中級レベルの具体的目標}

### 応用段階（該当する場合）
- {応用レベルの具体的目標}

## 評価基準
- {理解度を測る具体的な基準}
```

### 5. initial-concepts.md
```markdown
# 初期学習コンセプト

## コンセプト一覧
{学習範囲に基づいて抽出されたコンセプト}

## 依存関係
{コンセプト間の学習順序・依存関係}

## 推定学習時間
{各コンセプトの学習時間見積もり}
```

## 追加の推奨事項

### ディレクトリ構造の作成
```
/subjects/{学習分野名}/
├── metadata.md
├── scope-definition.md
├── knowledge-baseline.md
├── learning-objectives.md
├── initial-concepts.md
├── content/           # 今後生成される学習コンテンツ
├── assessments/       # 理解度テスト
└── progress/          # 学習進捗記録
```

### フォローアップ提案
対話完了後、以下を提案する：
- 「最初の学習セッションを開始しますか？」
- 「理解度テストを作成しますか？」
- 「学習スケジュールを立てますか？」

## 注意事項

1. **学習者のペースに合わせる**: 質問を一度にすべて投げかけず、対話的に進める
2. **具体例を求める**: 抽象的な回答には具体例を求めて明確化する
3. **範囲の調整**: 広すぎる場合は適切に絞り込みを提案する
4. **既存知識の活用**: 学習者の既存知識を最大限活用する学習プランを提案する
5. **柔軟性の確保**: 学習進行中に目標や範囲を調整できることを説明する

## 使用例

```
AIエージェント: 「新しい学習分野をセットアップしましょう。何について学びたいですか？」

学習者: 「LLMについて学びたいです」

AIエージェント: 「LLMについて、現在どの程度ご存知ですか？すでに理解している概念があれば教えてください」

[対話継続...]
```

---

この指示書に従って、学習者との対話を通じて適切な学習環境をセットアップしてください。