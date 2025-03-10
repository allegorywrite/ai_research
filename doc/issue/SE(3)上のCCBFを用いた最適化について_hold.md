# SE(3)上のCCBFを用いた最適化について（保留中）

## 提起された課題

実際のドローンのダイナミクスについて最適化を行うためには，SE(3)上でのダイナミクス表現や最適化を用いる必要があります．現在定式化しているCCBF付きMPCをリー群及びSE(3)上で再定式化してください。
リー群のCBFへの適用については一度サーベイを要求したほうが良いかもしれません。

## 保留理由

この課題は、リー群およびSE(3)上でのCBF/CCBFの定式化に関する専門的な知識を必要とします。現時点では、この分野に関する十分な情報がないため、まずはサーベイを実施することにしました。

サーベイリクエスト「リー群およびSE(3)上でのCBF/CCBFの定式化に関するサーベイ」（`doc/surveys/task_4/request.md`）を作成し、以下の点について調査を依頼しています：

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

## 今後の対応

サーベイの結果を待ち、リー群およびSE(3)上でのCBF/CCBFの定式化について理解を深めた上で、現在のCCBF付きMPC問題をSE(3)上で再定式化する予定です。特に、以下の点に注目して取り組む予定です：

1. SE(3)上でのドローンのダイナミクスモデルの定式化
2. SE(3)上でのCCBF制約の定義と性質
3. SE(3)上でのCCBF制約付きMPC問題の解法
4. 分散実装の可能性と計算効率の考慮

サーベイの結果が得られ次第、この課題に取り組み、SE(3)上でのCCBF付きMPC問題の定式化を行います。
