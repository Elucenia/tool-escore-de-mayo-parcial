<!-- ELUCENIA technical documentation · escore-de-mayo-parcial · zh · no clinical/professional/rights approval -->

# 部分 Mayo 评分（溃疡性结肠炎）

[条件、来源与许可](https://elucenia.org/zh/tools/escore-de-mayo-parcial)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 排便频率

`freq`

- `0` — 患者平常的排便次数
- `1` — 比平常多1至2次
- `2` — 多3至4次
- `3` — 多5次或以上

### 直肠出血

`sang`

- `0` — 无
- `1` — 少于一半的排便有血
- `2` — 一半或以上的排便有血
- `3` — 仅有血（无粪便）

### 医生总体评价

`global`

- `0` — 正常
- `1` — 轻度疾病
- `2` — 中度
- `3` — 重度

## 方法版本

部分Mayo/Lewis 2008：3项0–3，总分0–9，不含内镜

## 已记录的公式

排便频率（0至3）+ 直肠出血（0至3）+ 医生整体评估（0至3）。总分0至9。

完整Mayo（0至12）增加内镜表现（0至3）。

## 限制与适用人群

部分Mayo用于衡量溃疡性结肠炎的活动度与反应，包含三个项目而不含内镜；它不等同于完整Mayo，也不评估内镜愈合。Lewis2008在一项12周试验中分析了105例轻至中度疾病患者，将评分变化与患者感知的改善比较。这种设计不能证明它对重症、儿童或其他结肠炎普遍适用。请记录症状时段和医生评估；总分本身不能决定治疗。

## 参考文献

- [Schroeder KW, Tremaine WJ, Ilstrup DM. Coated oral 5-aminosalicylic acid therapy for mildly to moderately active ulcerative colitis: a randomized study. N Engl J Med, 1987.](https://doi.org/10.1056/NEJM198712243172603)

- [Lewis JD et al. Use of the noninvasive components of the Mayo score to assess clinical response in ulcerative colitis. Inflamm Bowel Dis, 2008.](https://doi.org/10.1002/ibd.20520)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

评分 ≤ 2：符合临床缓解

2.5 的截点对患者感知的缓解具有更好的敏感性和特异性（Lewis 2008）。


### 2

评分 ≥ 3：临床活动性疾病

较基线下降 3 分或以上提示临床应答（Lewis 2008）。


### 3

评分 ≥ 3：临床活动性疾病

较基线下降 3 分或以上提示临床应答（Lewis 2008）。

