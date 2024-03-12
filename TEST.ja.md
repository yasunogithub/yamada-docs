# Yamada-UI: Tips for Test

このドキュメントでは、Yamada-UIのテスト関連のtipsをまとめています。

## テスト実行方法

**全テスト実行**

```bash
pnpm test
```

**一つのコンポーネントのテスト実行**

```bash
pnpm test <component_name>

#例 Modalコンポーネントの場合
pnpm test modal
```

## テストカバレッジ確認方法

**ローカル環境**

1. `pnpm test:coverage`を実行
2. `http://localhost:4173/`にアクセス

## よくある質問

- 変更を加えた場合テストは追加すべきですか？

  - はい。ただ、誤記修正やドキュメント修正、コードの整理などの場合はテスト追加は不要です。

- テスト追加のみのPRの場合changesetファイルの追加は必要ですか？

  - 不要です。

- Codecobとはなんですか？
  - Yamada-Uiでは[Codecov](https://about.codecov.io/)を使用し、PR作成後テストカバレッジを可視化するようにしています。もし、Codecovについてwarningが出る場合は変更箇所のテストが行われていない可能性があります。そのため、テストが行われていない箇所を修正するか、テストの追加を行う必要があります。
