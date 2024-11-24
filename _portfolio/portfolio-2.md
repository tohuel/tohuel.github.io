---
title: "Quantile Instrumental Variable Panel Estimator"
excerpt: "Seminar paper written during my stay at ENSAE Paris Tech<br/><img src='/images/quantile_estimation.png'>
<br />
<br />
**Abstract**: 
This project critically reviews the evaluates the quantile regression dynamic panel data instrumental variables estimator (QRPIV) proposed by Galvao (2011). The method is summarised, main advances of the subsequent literature outlined and limitations of the Galvao (2011) approach assessed. 
We present a generic implementation of the estimator in R.
The suggested method to estimate dynamic quantile panel models is applied to the question of determinants of inflation dynamics. We find that inflation shows heterogeneity in persistence across quantiles.
"
collection: portfolio
category: econometrics
---

This paper critically evaluates the quantile regression dynamic panel data instrumental variables estimator (QRPIV) proposed by Galvao (2011) for addressing endogeneity in dynamic quantile panel models that include lagged dependent variables. Dynamic econometric models often incorporate lagged dependent variables to capture economic behaviors such as habit formation or inflation dynamics, where the impact of past values influences current outcomes. Quantile regression has emerged as a powerful tool to estimate such models while relaxing distributional assumptions. However, in panel data settings, controlling for endogeneity through fixed effects can cause bias, particularly when the panel dimensions are short. The estimator proposed by Galvao (2011), drawing on the methodology of Arellano (1991), is designed to mitigate this issue in the context of quantile regression.

The paper provides a detailed review of Galvao (2011) and highlights its significant but often overlooked limitations, especially the assumption that asymptotic properties hold when both cross-sectional and time dimensions are large. While the estimator is presented as a solution for short T panels, its derivation relies on large T assumptions, rendering it less effective in many practical applications, particularly when N exceeds T. The paper further demonstrates the technical challenges involved in implementing the estimator, including issues of stability in the case of unbalanced panels with large N and small T.

A critical contribution of the paper is the implementation of Galvao (2011)'s estimator in R, addressing the lack of a formal code base for this estimator. Despite the estimator's theoretical importance, it has not been widely adopted due to the absence of accessible code and difficulties in replication. The development of a generic R implementation of the estimator, which improves its accessibility and facilitates replication. 

The authors demonstrate the estimator's use in the context of inflation dynamics across advanced economies, illustrating its potential for empirical applications in macroeconomics. This implementation provides a crucial tool for researchers seeking to apply dynamic quantile regression models to panel data, thereby advancing the reproducibility of empirical research in economics.