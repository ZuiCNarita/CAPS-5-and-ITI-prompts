<!-- ------------------------------------------------------------

[ITI] Evaluation Introduction Prompts

------------------------------------------------------------ -->

<prompt id="introduce">
# カウンセリング会話ログについて

* 添付ファイル `*ITI_counseling_log.txt` は、International Trauma Interview (ITI) をベースとした、PTSD患者へのカウンセリングの会話ログです。
* カウンセリング会話ログ のフォーマット仕様を、添付の「ITI_counseling-log-prompts.md」に記載しています。

# カウンセリング会話ログの評点について

* カウンセリング会話ログに対する評点の採点の仕様を、添付の「ITI_replay-evaluate-prompts.md」に記載しています。
</prompt>

<!-- chatui からの入力の場合の、追加プロンプト -->
<prompt id="introduce-for-chatui">
* こちらから評点の出力開始指示があるまで、出力は待機してください。
</prompt>


<!-- ------------------------------------------------------------

Evaluation Prompts

* 基準パートごとの評点出力指示プロンプト

------------------------------------------------------------ -->

<prompt id="request_evaluate">
# 評点の開始指示

## 以下の基準（C-PTSD）の評点を出力してください
- "C-PTSD 基準 A"
- "C-PTSD 基準 B"
- "C-PTSD 基準 C"
- "C-PTSD 基準 D"
- "C-PTSD 全般的妥当性（C-PTSD 基準 A-D）"
</prompt>

<prompt id="request_evaluate_additional">
## 以下の基準（PTSD）の評点を出力してください
- "PTSD 基準 A"
- "PTSD 基準 B"
- "PTSD 基準 C"
- "PTSD 基準 D"
- "PTSD 基準 E"
- "PTSD 基準 F"
</prompt>

<prompt id="request_evaluate_summarize">
# 評点の集計指示

## 以下のサマリーを出力してください
### 基準（C-PTSD）の評点を、以下の表形式で出力してください
* フォーマット
  | 基準名 | 評点 |
  | -- | -- |
  | {基準名} | {評点} |
* 補足指示
  * 基準は C-9a C-9b など、明細まで出力してください
  * "C-PTSD 全般的妥当性" も出力対象としてください
### この患者に対するカウンセリングの総評を出力
* 総評は要約して出力してください
</prompt>

<prompt id="request_evaluate_summarize_additional">
## 以下のサマリーを出力してください
### 基準（PTSD）の評点を、以下の表形式で出力してください
* フォーマット
  | 基準名 | 評点 |
  | -- | -- |
  | {基準名} | {評点} |
</prompt>
