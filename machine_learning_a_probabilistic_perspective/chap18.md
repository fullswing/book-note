# State space models

## Introduction

状態空間モデル：HMMの隠れ状態が連続であるバージョン


$\boldsymbol{z}_t = g(\boldsymbol{u}_t, \boldsymbol{z}_{t-1},\boldsymbol{\epsilon}_t)$

$\boldsymbol{y}_t = h(\boldsymbol{z}_t, \boldsymbol{u}_t, \boldsymbol{\delta}_t)$

here
    
* $\boldsymbol{z}_t$ : hidden state
* $\boldsymbol{u}_t$ : an optional input or control signal
* $\boldsymbol{y}_t$ : the observation
* $g$ : transition model
* $h$ : observation model
* $\boldsymbol{\epsilon}_t$ : the system noise at time $t$

$\boldsymbol{\theta}$ : 全てのパラメータ

* すべてのパラメータが既知
* わからないパラメータがあるとき
    * すべては隠れ状態に含める


