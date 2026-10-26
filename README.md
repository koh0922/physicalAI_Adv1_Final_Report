PhysicalAI応用講座１の最終課題のNOTEBOOKデータなどを保管しています。
# PushT Policy Evaluation

## 概要

01_roboops_workshopをベースに、PushT Policyの学習と
Simulator上でのclosed-loop評価を行った。

## 目的

epochの増加、Datasetの各項目の品質改善のPolicyのsuccess rateに与える影響を調べる。

## 実装した工夫

- Dataset validatorを追加
- epochを複数パターン実施、効果を分析
- datasetの各項目の単独でのチェックおよび相互効果の検証

## 実行方法
#epoch数のパターン

1. 10 epoch
2. 30 epoch(Baseline)
3. 60 epoch
4. 120 epoch

#datasetの調整

1. REWARD
2. EPISODE LENGRH
3. ACTION SET
4. ACTION STATE DISTANCE 
5. STATIONARY RATIO
6. １−５の組み合わせでの相互効果

#追加

1. epoch数とdatasetの組み合わせで相互効果

## 結果

resul_sheet/に保管のspreadsheet参照
