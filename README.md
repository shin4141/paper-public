# Decision-OS V5 (SiriusA) — Paper Public Repo

**Scope**: 論文提出用の最小公開セット（原理/枠組み/図/匿名KPIのみ）。  
**Excludes**: 閾値・内部プロンプト全文・検知ロジック詳細・生ログ・個人情報。  
**Lineage**: Polaris → DGIS → SiriusA（系譜のみ記録、核は非公開）。  
**Ethics & Safety**: 非医療・2タップ手動・Human-in-the-loop・公開KPI（Adherence/Decision Time/FPR/FNR/Net Benefit/Brier/ECE）。  
**Submission plan**: arXiv（primary: cs.HC; cross: cs.AI/cs.CY）→ 査読誌（候補: HCI/HRI/Gerontechnology）。

## Layout
```
figures/       # 図（閾値や検知語の全文は記載しない）
appendices/    # 評価手順など（非個情・匿名）
audit/         # 版ログ（必要に応じてZIPやSHA）
main.tex
refs.bib
abstract.txt
teaser_150jp.txt
```

## Do-Not-Include (Hard Rule)
- 閾値の実数、内部プロンプト全文、検知語の具体列挙
- 生ログ・個人情報・識別可能なデータ
- private リポの内容への直リンク

## Build
- GitHub Actions で `main.tex` をビルドし、artifact としてPDFを確認可能。
- Overleaf Git 連携で編集する運用も想定（後述）。

## License
- 暫定: CC BY-NC-SA 4.0（変更の可能性あり）
