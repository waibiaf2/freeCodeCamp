---
id: 5900f5381000cf542c51004b
title: '問題 460: 歩き回るアリ'
challengeType: 1
forumTopicId: 302135
dashedName: problem-460-an-ant-on-the-move
---

# --description--

ユークリッド平面上で、アリが点 $A(0, 1)$ から点 $B(d, 1)$ へ移動します。ここで、$d$ は整数です。

各ステップにおいて、点 ($x_0$, $y_0$) にいるアリは、$x_1 ≥ 0$, $y_1 ≥ 1$ を満たす格子点 ($x_1$, $y_1$) のうち 1 つを選び、一定の速度 $v$ で ($x_1$, $y_1$) に向かって直進します。 $v$ の値は、$y_0$ と $y_1$ によって次のように決まります。

- $y_0 = y_1$ の場合、$v$ の値は $y_0$ に等しい。
- $y_0 ≠ y_1$ の場合、$v$ の値は $\frac{y_1 - y_0}{\ln y_1 - \ln y_0}$ に等しい。

左側の図は、$d = 4$ の場合に考えられる経路の一つです。 まず、アリは $A(0, 1)$ から $P_1(1, 3)$ まで、速度 $\frac{3 - 1}{\ln 3 - \ln 1} ≈ 1.8205$ で進みます。 したがって、所要時間は $\frac{\sqrt{5}}{1.820} ≈ 1.2283$ です。

$P_1(1, 3)$ から $P_2(3, 3)$ までは速度 3 で移動するので、所要時間は $\frac{2}{3} ≈ 0.6667$ です。 $P_2(3, 3)$ から $B(4, 1)$ までのアリの移動速度は $\frac{1 - 3}{\ln 1 -\ln 3} ≈ 1.8205$なので、所要時間は $\frac{\sqrt{5}}{1.8205} ≈ 1.2283$ となります。

したがって、合計所要時間は $1.2283 + 0.6667 + 1.2283 = 3.1233$ です。

右側の図は別の経路です。 合計所要時間は $0.98026 + 1 + 0.98026 = 2.96052$ となります。 これが $d = 4$ に対する最速経路であることが分かっています。

<img alt="d = 4 に対して考えられる経路" src="https://cdn.freecodecamp.org/curriculum/project-euler/an-ant-on-the-move.jpg" style="background-color: white; padding: 10px; display: block; margin-right: auto; margin-left: auto; margin-bottom: 1.2rem;" />

アリが最速経路を選んだ場合の合計所要時間を $F(d)$ とします。 例えば、$F(4) ≈ 2.960\\,516\\,287$ です。 $F(10) ≈ 4.668\\,187\\,834$, $F(100) ≈ 9.217\\,221\\,972$ であることを確認できます。

$F(10\\,000)$ を求めなさい。 回答は、四捨五入して小数第 9 位まで示すこと。

# --hints--

`antOnTheMove()` は `18.420738199` を返す必要があります。

```js
assert.strictEqual(antOnTheMove(), 18.420738199);
```

# --seed--

## --seed-contents--

```js
function antOnTheMove() {

  return true;
}

antOnTheMove();
```

# --solutions--

```js
// solution required
```
