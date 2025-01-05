# daily-commit

このリポジトリは、GitHub Actionsを利用して毎日自動的にコミットを行う仕組みを提供します。

## 仕組み

- **GitHub Actions**を使用して、指定した時間にスケジュールされたタスクを実行します。
- 日付と時刻を含むログを`commit-log.txt`に記録します。
- 毎回のログは日本時間（JST）で記録されます。

## 使用方法

1. **リポジトリのクローン**:
  ```bash
  git clone https://github.com/busaiku0084/daily-commit.git
  ```

2. **commit-log.txt の確認**:
  - 最新の自動コミットログが記録されています。

3. **スケジュール変更**:
  - `.github/workflows/daily-commit.yml`内の`cron`値を変更することで、スケジュールを調整できます。

## ログファイル構成

- `commit-log.txt`には以下のフォーマットでログが記録されます:
  ```txt
  Auto commit on 2025-01-10 08:00:00 JST
  Auto commit on 2025-01-11 08:00:00 JST
  ```
