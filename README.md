# 社保实缴前后测算表

算一件事：**我的社保缴费基数比实际工资低，每月要补多少钱？**
填进去工资和现在的缴费基数，养老 / 医疗 / 失业三个险种的单位侧、个人侧差额即时算出来，还能看一条「工资 → 每月补缴」的变化曲线。

[打开工具 →](https://abububu903.github.io/shebao-calc/) · [English](#english)

---

## 打开就用

👉 **[abububu903.github.io/shebao-calc](https://abububu903.github.io/shebao-calc/)**

不用安装、不用注册，手机浏览器也能打开。想本地跑：下载 `index.html` 双击打开即可（纯前端，没有后端）。

## 一个例子

实际工资 12000 元/月，单位按 6000 元基数缴 →
把「实际工资」填 12000、「现缴费基数」填 6000，切到「综合」，
结果区直接给出**每月要补（元）**，并拆成单位侧 / 个人侧两行，以及每个险种各自的差额。

## 数据怎么查

「实际工资」请查个税 APP 的收入，「现单位/个人缴费额」请微信搜索「我的社保卡-个人服务查询-社保缴费信息查询」，工具不记录任何数据，放心使用

## 数据口径

默认26年深圳基数，基数上下限按当地当年为准，可自行修改

其他城市的用法：把「基数下限」「基数上限」两栏改成当地当年公布的数值即可，比例也能改。

## 免责

作者：abububu903 ｜ 结果仅供参考，以社保经办机构核定为准

## 文件说明

| 文件 | 作用 |
| --- | --- |
| `index.html` | 工具本体，页面 + 样式 + 计算逻辑全在这一个文件里 |
| `README.md` | 你正在看的这个说明页，GitHub 自动展示在仓库首页 |

## 已知边界

- 只算**养老 + 医疗 + 失业**三项，工伤/生育和公积金不在范围内
- 补缴金额按线性差额估算，实际核定可能涉及滞纳金、基数核定口径等，本工具不覆盖

---

## English

A one-page calculator for a very specific question: **my employer declares a lower social-insurance base than my real salary — how much should be topped up each month?**

Enter your actual monthly salary and the base currently used. The tool computes the shortfall for the three mandatory schemes (pension, medical, unemployment), split into employer-side and employee-side, and plots a salary → monthly-top-up curve.

- **Live page:** <https://abububu903.github.io/shebao-calc/> — no install, no sign-up, works on mobile. Or download `index.html` and open it directly; it is pure frontend with no backend.
- **Defaults:** Shenzhen 2026 contribution bases. The lower/upper base limits and the rates are editable, so the same page works for other cities.
- **Privacy:** nothing is stored or sent anywhere. All computation happens in your browser.
- **Scope:** pension + medical + unemployment only. Maternity, work-injury and the housing fund are out of range. Figures are linear estimates — the final assessment belongs to the local social-insurance authority.

*By abububu903. Results are for reference only.*
