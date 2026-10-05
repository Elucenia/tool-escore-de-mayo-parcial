<!-- ELUCENIA technical documentation · escore-de-mayo-parcial · ja · no clinical/professional/rights approval -->

# 部分Mayoスコア（潰瘍性大腸炎）

[条件・出典・許諾](https://elucenia.org/ja/tools/escore-de-mayo-parcial)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 排便回数

`freq`

- `0` — 患者の通常の状態
- `1` — 通常より1～2回多い
- `2` — 3～4回多い
- `3` — 5回以上多い

### 直腸出血

`sang`

- `0` — なし
- `1` — 排便の半分未満に血液がある
- `2` — 排便の半分以上に血液がある
- `3` — 血液のみ（便なし）

### 医師による全般評価

`global`

- `0` — 正常
- `1` — 軽症
- `2` — 中等度
- `3` — 重度

## 方法の版

部分Mayo/Lewis 2008：3項目0–3、合計0–9、内視鏡なし

## 記載された計算式

排便頻度（0～3）+ 直腸出血（0～3）+ 医師総合評価（0～3）、合計0～9。

完全Mayo（0～12）は内視鏡所見（0～3）を加えます。

## 限界・対象集団

部分Mayoは、三項目で内視鏡を含まず、潰瘍性大腸炎の活動性と反応を測定します。完全Mayoと同等ではなく、内視鏡的治癒を評価しません。Lewis2008は12週間の試験で軽度から中等度の105例を解析し、変化を患者が感じた改善と比較しました。この研究デザインは、重症例、小児、その他の大腸炎での普遍的性能を示しません。症状の期間と医師の評価を記録してください。合計点だけで治療は決まりません。

## 参考文献

- [Schroeder KW, Tremaine WJ, Ilstrup DM. Coated oral 5-aminosalicylic acid therapy for mildly to moderately active ulcerative colitis: a randomized study. N Engl J Med, 1987.](https://doi.org/10.1056/NEJM198712243172603)

- [Lewis JD et al. Use of the noninvasive components of the Mayo score to assess clinical response in ulcerative colitis. Inflamm Bowel Dis, 2008.](https://doi.org/10.1002/ibd.20520)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026
