ccbfが今回の問題に適しているようなのはわかったが，視野の共有判定もしくは制約の定式化について疑問がある．
1. 環境内の特徴点（ランドマーク）が複数のUAVによって同時に観測されることを保証したいとあるが，agent 1が観測しているすべての特徴点を他のエージェントが観測することは不可能である．目的はあくまで協調自己位置推定が達成されることで，推定のために十分な特徴点の共有があれば良いはずである．
2. 更にいえば，交差制約を距離と角度のみによって判定しているが，実際にはオクルージョンが存在し，上記の制約が満たされていても視野を共有できていない状況が存在し得るため，距離と角度のみによる制約は完璧とはいえないはずである．オクルージョン平面からの距離を含むような文献もあったはずであるが，ここに関しての深耕は必須であろう．
3. 現在の研究進捗においては目的関数が目標状態誤差と入力のような形式になっているが，上記1の指摘を鑑みれば，そもそも自己位置推定における最適問題に基づいた定式化もあり得るはずである．この定式化に基づいた理論研究もまとめてもらいたい．適宜サーベイの必要があればまとめるべし．