# 中英書房 · en-biz

繁體中文 ⇄ English 的單頁翻譯工具，提供：

- 中文草稿轉成可直接整理寄出的國際商務英文郵件
- 中文寄信郵件完成後可自動潤稿（預設開啟，可在設定中關閉）
- 英文來信翻成台灣繁體中文
- 面對面中英口譯與譯文朗讀
- 反譯、商務潤稿、字彙表與選字問 AI

本專案為純前端靜態頁面。OpenAI API Key 與選用的 Google Cloud TTS Key 由使用者在瀏覽器本機設定。

## 使用

線上使用：<https://kenkenno1.github.io/en-biz/>

本機開啟 `index.html` 即可使用；`index.html` 與 `中英學習軟體.html` 為同一份發布內容。

版本：v1.3.0

v1.2.0：字彙表的 AI 抽取支援短文、單次出現的重要單字與片語，並以原文存在性 gate 防止候選詞捏造。

v1.3.0：模型升級為 GPT-5.6（預設 `gpt-5.6`，成本平衡 fallback `gpt-5.6-terra`）；使用者選定模型優先於上次成功模型。字彙抽取改為跨 chunk rank round-robin、每次全域最多 20 組，並強化英文完整 token、智慧引號與 dash 變體比對。

## 品牌圖示

`assets/en-biz-logo-v1.png` 為中英書房的高解析 Logo 原圖；PWA、Apple touch icon 與 favicon 均由此圖衍生。
