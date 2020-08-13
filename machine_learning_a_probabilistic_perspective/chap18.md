# State space models

## Introduction

状態空間モデル：HMMの隠れ状態が連続であるバージョン


$$\boldsymbol{z}_t = g(\boldsymbol{u}_t, \boldsymbol{z}_{t-1},\boldsymbol{\epsilon}_t)$$

$$\boldsymbol{y}_t = h(\boldsymbol{z}_t, \boldsymbol{u}_t, \boldsymbol{\delta}_t)$$

where
    
$$\boldsymbol{z}_t \text{ : hidden state}$$
$$\boldsymbol{u}_t \text{ : an optional input or control signal}$$
$$\boldsymbol{y}_t \text{ : the observation}$$
$$g \text{ : transition model}$$
$$h \text{ : observation model}$$
$$\boldsymbol{\epsilon}_t\text{ : the system noise at time $t$}$$

$\boldsymbol{\theta} \text{ : all parameters}$

* すべてのパラメータが既知
* わからないパラメータがあるとき
    * すべては隠れ状態に含める


