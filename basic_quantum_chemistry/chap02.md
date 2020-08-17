# 波動性と粒子性

ボーアの量子条件の物理的な背景

## 光の波動性

### 光は波動性と粒子性をあわせもつ。もっというと、粒子として存在している物質も、ある条件下では波として振舞う。

実験事実

* ヤングの二重スリット実験
    * 光は干渉して強めあったり、弱めあったりする（波動性）

## 光の粒子性

実験事実

- 光電効果
    - 物質が光を吸収して電子を放出する現象。
        1. ある振動数 $\nu_0$ より低い振動数 $\nu$ の光では、光の強度を強くしても光電効果は起きない。
        2. 照射する光の振動数 $\nu$ が $\nu_0$ を超えて大きくなると、放出される光電子のエネルギー $E_p$ は $\nu-\nu_0$ に比例して大きくなる（光子のエネルギーは $\nu$ に比例して大きくなる）。

- 光が波だと仮定すると、以下の点で矛盾から実験事実に反する。
    - 光が波であると考えると、光の強度は波の振幅の2乗に比例する。→ [Link](https://eman-physics.net/dynamics/wave_energy.html)
    - 物質が受け取るエネルギーも振幅の2乗に比例するならば、低い振動数の光でも強度さえ強くすれば光電効果が起こってもよいはず

1個の光子が物質によって吸収され、その結果1個の電子が物質から放出されるとする。1個の光子のエネルギーは $h\nu$ で与えられる。

放出されたエネルギー $E_p$ は、以下の式で表される。

$$E_p = h\nu - W$$

ここで、$W$ は結合エネルギー。$E_p \geq 0$ なので、$h\nu \geq W$ でなければならない。したがって、光電効果が起こるための振動数の閾値は以下で与えられる。

$$\nu_0 = \frac{W}{h}$$

また、光電子のエネルギーは以下で表される。

$$E_p = h(\nu-\nu_0)$$

## 光の粒子性と波動性

相対性理論より、

\begin{align}
    m_v &= \frac{m_0}{\sqrt{1-\frac{v^2}{c^2}}} \cdots \text{ ①}\\
    E &= m_vc^2 \\
    \therefore \text{ } E^2 &= {m_0}^2c^4 + p^2c^2
\end{align}

ここで、$p$ は光子の運動量であり、$p=m_vv$ である。上で $m_0=0$ とすると、

\begin{align}
    E &= pc \\
      &= h\nu \\
      &= h\frac{c}{\lambda} \\
    \therefore \text{ } p &= \frac{h}{\lambda}
\end{align}

## 電子の粒子性と波動性

* 粒子性
    * 電子は負の電荷を帯びた粒子である。
    * 電子を1個ずつ検出できることから明らか
* 波動性
    * 電子をしばらく検出し続けると検出板の上に明暗のパターンが現れる


## 物質波とド・ブロイの式

### 粒子として存在している物質も、ある条件下では波として振舞う

速度 $v$ で運動している質量 $m$ の粒子は

$$\lambda = \frac{h}{mv} = \frac{h}{p}$$

## 物質波とボーアの量子条件

#### ボーアの量子条件

$$mvr = n \frac{h}{2\pi}$$

これとド・ブロイの式をあわせると

$$2\pi r = n \lambda$$

円軌道の円周の長さが電子のド・ブロイ波長の整数倍になっている。

#### ボーアの量子条件は、電子のド・ブロイ波が定在波（空間の波形が時間経過で変化しない）になる条件である。

## 波動方程式

目標 : 一次元の波動方程式を導く→波動方程式を解く→シュレーディンガー方程式を導出する

### 一次元の波動方程式を導く

振幅が$x, t$ に依存するので、$x$ と$t$ の二階微分を結びつける。

$$\frac{\partial^2 u}{\partial x^2} = \frac{1}{v^2}\frac{\partial^2 u(x,t)}{\partial t^2}$$

$u$ : $x$ 軸からの変位

$t$ : 時間

$l$ : 弦の長さ. $x \ll l$

#### 方針

1. 位置$x$ を中心として、長さd$x$ の弦の微小部分の運動方程式を考える。
2. 微小成分・微小角に注目して近似
3. 微分の定義に戻る

バネの密度を $\rho$ とする。加速度は振幅を時間 $t$ で二階微分したものなので、運動方程式 $ma=F$ の左辺は以下で表される。

$$ma=\rho \text{ d}x \frac{\partial^2 u}{\partial t^2}$$

次に、バネの微小区間にかかる張力のうち、加速度にかかわる垂直方向の成分のみを考える。

$$F = T(\sin \theta_1-\sin \theta_2)$$

$x \ll l$ なので、$\theta_1, \theta_2$ も十分に小さいとしてよい。すなわち、$\sin \theta_1 \approx \tan \theta_1$ のように近似できる。ここで、$\tan \theta_1 = (\frac{\partial u}{\partial x})_{x+\frac{d}{2}},\tan \theta_2 = (\frac{\partial u}{\partial x})_{x-\frac{d}{2}}$ なので、

\begin{align}
    F &= T(\sin \theta_1-\sin \theta_2) \\
      &\approx T(\tan \theta_1-\tan \theta_2) \\
      &= T\{(\frac{\partial u}{\partial x})_{x+\frac{d}{2}}-(\frac{\partial u}{\partial x})_{x-\frac{d}{2}}\} \\
      &= T\frac{(\frac{\partial u}{\partial x})_{x+\frac{\text{d}x}{2}}-(\frac{\partial u}{\partial x})_{x-\frac{\text{d}x}{2}}}{\text{d}x}\text{d}x \\
      &= T \frac{\partial^2 u}{\partial x^2}\text{d}x \\
\end{align}

これらを $ma=F$ に代入すると、

\begin{align}
    \rho \text{ d}x \frac{\partial^2 u}{\partial t^2} &= T \frac{\partial^2 u}{\partial x^2}\text{d}x \\
    \therefore \text{ } \frac{\partial^2 u}{\partial x^2} &= \frac{\rho}{T} \frac{\partial^2 u(x,t)}{\partial t^2} 
\end{align}

$v = \sqrt{\frac{T}{\rho}}$ とおけば、以下の波動方程式が得られる。

$$\frac{\partial^2 u}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 u(x,t)}{\partial t^2}$$

### 波動方程式を解く

#### 目的

ある時間 $t$ 、ある位置 $x$ における変位 $u$ がいくつか、つまり $u(x,t)$ を求めること。

#### 方針

1. 条件を洗い出す
2. 変数を分離する
3. それぞれの変数について方程式を導出する
4. 場合分けしてそれぞれの変数について解を求める
5. まとめる

### $v$ の意味

#### 目標 

波長と振動数の積は波の速度になる。

$$v = \lambda_n \nu_n$$

### 二次元の波動方程式

