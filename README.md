# aws-hikinou-grade
IPAの作成している **[「非機能要求グレード」](https://www.ipa.go.jp/sec/softwareengineering/std/ent03-b.html)** を参考にして AWS利用時に非機能要求を整理するための道具  
非機能要求グレードはそこそこ細かいため簡潔に実施可能なように要点をまとめる  
また [AWS Well-Architected](https://aws.amazon.com/jp/architecture/well-architected/) も取り入れる予定  

## 非機能要求グレード とは  

* システムの稼働率や性能目標、災害時の復旧時間、セキュリティ対策方針などの「非機能」に関する要求を可視化するための表
  * システムに求める「機能」の一覧は定義しやすいものの 「非機能」の一覧については定義が難しい、または定義していないも多かったため可視化するために出来た道具

## aws-hikinou-grade 説明

* 「分割」フォルダ配下のファイル
  * 下の「tmp--非機能要求グレード活用シート_AWS編.xlsx」を MarkDown に変換し AWS環境 での非機能を設計するために用語や記載内容を改め分割したもの
    * 1-セキュリティ.md
    * 2-可用性.md
    * 3-性能・拡張性.md
    * 4-運用・保守性.md

* tmp--非機能要求グレード活用シート_AWS編.xlsx
  * **[「非機能要求グレード」](https://www.ipa.go.jp/sec/softwareengineering/std/ent03-b.html)** に梱包している「06_活用シート.xls」を色付けした一時ファイル
    * 構築に関わるもの→水
    * 運用に関わるもの→緑
    * 移行に関わるもの→橙
    * AWSでは不要なもの→灰
