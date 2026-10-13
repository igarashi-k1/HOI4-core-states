# Core Controlled States (HOI4 MOD)

ディシジョンを選択すると、自国が保有または支配（占領含む）しているステートをすべて中核州にします。

| ディシジョン | 効果 |
| --- | --- |
| 支配ステートをすべて中核州にする | 保有・支配しているステートのうち、まだ中核州でないものすべてに自国の中核を追加 |

- 政治力コスト 0、何度でも実行可能（中核化できるステートがない間は実行不可）
- AI は使用しません（`ai_will_do = 0`）
- 占領地の所有者は変わりません（中核だけが付与されます）

## インストール

1. このリポジトリを `Documents/Paradox Interactive/Hearts of Iron IV/mod/core_states/` に配置
2. 同じ `mod` フォルダに `core_states.mod` を作成し、以下を記述

```
version="1.0.0"
tags={
	"Gameplay"
}
name="Core Controlled States"
supported_version="1.*"
path="mod/core_states"
```

3. ランチャーで MOD を有効化

## 構成

```
descriptor.mod
common/decisions/categories/core_states_categories.txt
common/decisions/core_states_decisions.txt
localisation/english/core_states_l_english.yml   (UTF-8 BOM付き)
localisation/japanese/core_states_l_japanese.yml  (UTF-8 BOM付き)
```

※ ローカライズは `l_japanese`（ゲームの言語設定が日本語の場合）と `l_english`（英語設定＋日本語化MODの場合）の両方に日本語で記述しています。
