# qa-docx-converter
Simple Python3 tool for converting .csv file into a Q & A .docx file.

## notes
- .csv file must contain at least one title, one question and one or several answers.
- You must set parameters in config.ini.

## QA用.docx作成ツール仕様
CSVファイルに含まれる「見出し」「質問」「回答」をWordファイルに転記します。

- CSVファイルは、当pyファイルと同一ディレクトリ内に存在すること、パラメータ設定「config.ini」も同ディレクトリ内に存在すること、Wordファイルも、同ディレクトリ内に作成or上書きされることを想定しています。
- CSVファイル1行につき1つの質問、質問に対する回答は1〜n回分あることを想定しています。
- Wordファイルに転記する回答は「最終回答」のみとします。
- 1見出し/質問/回答を出力後に改ページします。
- 「見出し」のスタイルは0:Title固定、「質問」「回答」(小見出し)のスタイルは1:Heading 1固定、「質問」「回答」の内容自体はスタイル指定なしとします。
- Title、Heading 1の書式はWord側で適宜編集してください。
- config.iniにファイル名、列インデックスを指定してください。
