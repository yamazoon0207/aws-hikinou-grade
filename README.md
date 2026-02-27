# aws-hikinou-grade

IPAが提供する **[「非機能要求グレード」](https://www.ipa.go.jp/sec/softwareengineering/std/ent03-b.html)** をベースに、AWS環境における非機能要求を整理するためのツールです。  
非機能要求グレードは項目が細かいため、実務で使いやすいよう要点を絞ってまとめています。  
また、[AWS Well-Architected](https://aws.amazon.com/jp/architecture/well-architected/) のベストプラクティスも取り入れる予定です。

## 非機能要求グレードとは

システムの稼働率、性能目標、災害時の復旧時間、セキュリティ対策方針など、「非機能要件」を可視化するためのフレームワークです。

機能要件は一覧化しやすい一方で、非機能要件は定義が難しく、見落とされがちです。このフレームワークを使うことで、非機能要件を漏れなく整理できます。

## 構成

### 「分割」フォルダ

「tmp--非機能要求グレード活用シート_AWS編.xlsx」をMarkdown形式に変換し、AWS環境に合わせて用語や内容を調整したファイル群です。

* 1-セキュリティ.md
* 2-可用性.md
* 3-性能・拡張性.md
* 4-運用・保守性.md

### 「AIエージェント用」フォルダ

aws-presales-playbookから非機能要件に関する内容（BANTC以外）を抽出したナレッジベースです。  
AIエージェントがAWS案件のプリセールス活動で参照することを想定しています。

* presales-aws-nonfunctional.md - AWS非機能要件の全体概要
* presales-security.md - セキュリティ要件
* presales-availability.md - 可用性要件
* presales-performance.md - 性能・拡張性要件
* presales-operability.md - 運用・保守性要件
* presales-compliance.md - コンプライアンス要件
* presales-cost.md - コスト最適化要件

### tmp--非機能要求グレード活用シート_AWS編.xlsx

**[「非機能要求グレード」](https://www.ipa.go.jp/sec/softwareengineering/std/ent03-b.html)** に含まれる「06_活用シート.xls」に色付けした作業用ファイルです。

* 構築に関わる項目 → 水色
* 運用に関わる項目 → 緑色
* 移行に関わる項目 → 橙色
* AWSでは不要な項目 → 灰色
