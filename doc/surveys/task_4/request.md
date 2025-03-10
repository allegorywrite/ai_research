# リー群およびSE(3)上でのCBF/CCBFの定式化に関するサーベイ

## 背景

現在、複数UAVによる協調的visual-inertial SLAMシステムにおいて、Consensus-Based Control Barrier Function (CCBF)を用いた視野錐台交差制約付きMPC問題の研究を進めています。これまでの研究では、ドローンのダイナミクスを一般的な非線形状態空間モデルとして定式化し、CCBF制約付きMPC問題を解く方法を検討してきました。

しかし、実際のドローンのダイナミクスをより正確に表現するためには、SE(3)上でのダイナミクス表現や最適化を用いる必要があります。特に、ドローンの姿勢は回転行列やクォータニオンで表現され、これらはSE(3)やSO(3)などのリー群に属します。通常のユークリッド空間での最適化手法をそのまま適用することはできないため、リー群上での最適化手法が必要となります。

## サーベイ内容

以下の点について、最新の研究成果や手法をサーベイしてください：

1. **リー群上でのCBF/CCBFの定式化**
   - リー群（特にSE(3)やSO(3)）上でのCBFの定義と性質
   - リー群上でのCBFを用いた制御設計の方法
   - リー群上でのCCBFの拡張と分散実装の可能性

2. **SE(3)上でのMPC問題の定式化と解法**
   - SE(3)上でのMPC問題の定式化（目的関数、制約条件など）
   - SE(3)上での最適化アルゴリズム（リーマン多様体上の最適化など）
   - 計算効率とリアルタイム実装の考慮事項

3. **SE(3)上でのCBF/CCBF制約付きMPC**
   - SE(3)上でのCBF制約をMPC問題に組み込む方法
   - SE(3)上でのCCBF制約付きMPC問題の分散解法
   - 実装例や実験結果（もしあれば）

4. **ドローンの制御への応用**
   - SE(3)上でのCBF/CCBFを用いたドローンの制御例
   - 視野制約や衝突回避などの安全制約の組み込み方
   - 複数ドローンの協調制御への応用

## 期待される成果

このサーベイを通じて、リー群およびSE(3)上でのCBF/CCBFの定式化と、それを用いたMPC問題の解法について理解を深めたいと考えています。特に、現在の研究テーマである「複数UAVによる協調的visual-inertial SLAMシステムにおける視野錐台交差制約付きMPC問題」をSE(3)上で再定式化するための理論的基盤を得ることを目指しています。

また、リー群上でのCBF/CCBFの定式化が、従来のユークリッド空間での定式化と比較してどのような利点や課題があるのかについても知りたいと考えています。
