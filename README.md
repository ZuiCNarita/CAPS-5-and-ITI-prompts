- プロンプトは以下で構成される
  1. カウンセリングログのフォーマット仕様を指示したプロンプトファイル
      - (CAPS5|ITI)_counseling-log-prompts.md
  2. 評価の仕様を指示したプロンプトファイル
      - (CAPS5|ITI)_replay-evaluate-prompts.md
  3. 処理の実行を指示するプロンプトファイル
      - (CAPS5|ITI)_replay-evaluate-prompts-intro.md
- カウンセリングログファイル＋プロンプトテキストを、プログラム（Pythonなど）を使用し、AIモデルへ投入する
  - プログラム実行環境は、以下を想定
    - Gemini処理実行: Google Colabo
    - Claude処理実行: Google Colabo 、または任意のPC環境
