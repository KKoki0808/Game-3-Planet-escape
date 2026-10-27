> Publication scope update (2026-10-27): This file is part of a documentation-only publication. References below to pending publication concern the full Unity project, media and Windows game, or earlier preparation steps. See [PUBLICATION_STATUS.md](PUBLICATION_STATUS.md) for current scope. No underlying media is included.

# AME294 Game 3：公開準備の最終判定

確認日：2026-10-27。ユーザー確認：本人生成、Tripo／ElevenLabsとも生成時Free、非商用の大学課題。ゲーム・SpaceSalvageRun・既存Windowsビルドは変更しない。許諾未確認の公開は実施しない。

## 先に公開候補にできるもの

文書のみ：README.md、PROMPT_LOG.md、ASSET_CREDITS.md、ASSET_RIGHTS_REVIEW.md、ASSET_LICENSE_INVENTORY.csv、PUBLICATION_STATUS.md、THIRD_PARTY_NOTICES.md、本書、問い合わせ文案、Release文案、ファイル別判定CSV、パッケージの原ライセンス／NOTICE文書。素材そのものは含めない。過去プロンプトは存在する制作記録を維持し、欠落を創作しない。文書に記載されたモデル名や素材パスは素材データの配布とは別。

文書のみの公開用コピー・ZIP・SHA256一覧を `Temp/PlanetEscape_DocsReady_20261027/` と `Temp/PlanetEscape_DocsReady_20261027.zip` に用意する。対象は許可リスト限定で、隠しGit履歴、モデル、画像、音声、シーン、ビルドを含めない。公開候補文書のローカルパス・秘密情報パターンを検査する。これは文書公開の準備でありGitHub掲載済みという意味ではない。

## ソースとビルドの別判定

| 対象 | GitHub素材ソース | Windows組み込み配布 | 理由・残る確認 |
| --- | --- | --- | --- |
| A01–A21 Tripo Free本人生成モデル | 保留 | 非商用利用の裏付けあり。無料出力の組み込み配布範囲の確認待ち | T：料金表の非商用利用と規約3.2は利用を支持するが、5.2.1の権利留保の下での原本・派生物再配布を明確に確定できない |
| A22–A29 ElevenLabs Free本人生成効果音 | MP3単体配布は制限対象。例外許諾なしに公開しない | 組み込みゲームは条件付き可 | E：非商用、指定タイトル帰属表記等。既存バイナリを変えず公開ページのタイトル・READMEで足りるか確認 |
| A30 生成空画像 | 入力権利の根拠確認待ち | 同左 | O：生成出力の権利は支持されるが、参考写真の入力権利を付与するものではない |
| A31 参考写真 | 除外維持 | 実行時不使用 | R：出典・許諾未記録。今回配布しない |
| 自作コード・設定・シーン | 本件の素材レビューだけで全体許諾済みとはしない | ゲーム内容は維持 | ソース公開する場合は素材埋め込みや参照を別途確認。本パッケージには含めない |
| 完成済みPlanetEscape_Windows64.zip | ソースではない | 上記T/E/O条件が解決するまで保留 | 原本が見えなくても派生メッシュ・テクスチャ・音声を内包する |

31件の個別パス・元名・SHA256・3用途の判定は [ASSET_LICENSE_INVENTORY.csv](ASSET_LICENSE_INVENTORY.csv)。原本に加えてモデル各フォルダの派生メッシュ・FBX・テクスチャ・マテリアル、音声メタ、空関連を[PUBLICATION_FILE_DECISIONS.csv](PUBLICATION_FILE_DECISIONS.csv)にファイル単位で列挙した。派生物の親フォルダによる保守的な列挙であり、全ファイルが法的に同一性を持つと断定するものではない。別フォルダに埋め込まれた派生データが存在しないことの証明でもない。今回の公開用コピーは文書のみの許可リストなので、そうした見落としに依存しない。

## 公式根拠（本日再取得）

- [Tripo規約](https://www.tripo3d.ai/terms)3.2／5.2.1（更新2025-07-11）と[料金表](https://www.tripo3d.ai/pricing)。Freeの非商用利用は確認できる。Unityソースの一般公開を明示的に許諾する条項は確認できない。「公開モデル」という表示を無制限の再配布ライセンスに置き換えない。
- [Tripo公式ヘルプ](https://www.tripo3d.ai/help/privacy-policy/how-to-use-tripo-models-commercially)もFreeの権利留保を説明。非商用の本人利用と、原本の再配布・受領者への再許諾を区別する。無料出力に未確認のCCライセンスを付けない。
- [ElevenCreative Terms](https://elevenlabs.io/creative-terms)Exhibit 4 §2（更新2026-10-09）：ゲーム等の複合制作物への利用と、孤立した音声ファイルの提供を区別。一般GitHub公開は公式Community Sharingの例外と同じではない。
- [ElevenLabs公式公開ガイド](https://elevenlabs.io/docs/help-center/legal/can-i-publish-the-content-i-generate-on-the-platform)：Freeは非商用、タイトルに `elevenlabs.io` または `11.ai` の表記が必要。READMEのクレジットだけでタイトル条件を代替したとは扱わない。

## MP3を単体公開しない具体策

現在のmainをそのままPushしない。現在の履歴にはMP3やモデルが既に含まれ、後から.gitignoreに追加したり削除コミットを作ったりしても履歴から取得できる。Git LFSへ置くだけでも配布自体は解消しない。

最短案は、原プロジェクトと既存Git履歴を保存し、**文書のみの独立した公開用履歴**から公開すること。完全ソースが課題上必要なら、音声・未許諾モデルのないソースが許されるか担当教員へ確認する。コードだけなら完全に再構築できるとは書かない。既存ビルドが許諾条件を満たした後は、通常のUnityゲームとして埋め込みのままZIPを配布し、音源フォルダ・単体音声の別ダウンロードを用意しない。拡張子変更・暗号化・LFSで規約を回避する案ではない。

## 最短の提出手順

1. 今すぐできる準備：文書パッケージとファイル別保留一覧は作成済み。公開用README・Release文案には11.aiを含むタイトルを設定した。元ゲームのタイトルやバイナリは変更していない。
2. 教員の課題要件を確認する。ここには採点基準の原文がないため、文書のみのURLで提出条件を満たすとは断定できない。期限が先なら、文書URLと「実行版は配布条件確認中」という現状の提出が認められるか相談する。
3. Tripoへ、非商用Windows組み込み配布とUnity原本／派生物の公開可否を分けて一括照会。ElevenLabsへ、既存バイナリを変更せず外部のReleaseタイトルとREADMEで帰属表記を満たせるか照会。英文はLICENSE_INQUIRIES.mdに用意済み。送信していない。
4. 参考写真の出典・入力利用の根拠が分かれば記録する。本人撮影か、適用ライセンス等を確認する。生成画像を無断複製と決めつける意味ではない。回答がなければ許諾済みとしない。
5. 文書公開を実行する際は、リモートの現状を再取得する。空なら文書のみの新しい公開履歴から通常Pushし、空でなければ既存履歴を尊重して統合する。原プロジェクトのmainを強制Pushしたり書き換えたりしない。今回は公開操作を実行しない。
6. ビルド配布条件が解決したら、`RELEASE_DRAFT.md` の公開タイトルを使用して**既存ZIPをそのまま**添付する。公開前後にSHA256を照合し、その後READMEへ実在するReleaseダウンロードURLを追記する。

現時点で準備完了なのは文書であり、完全Unityソース公開・Windows公開が完了したとは報告しない。問い合わせへの返答や教員の判断を創作せず、無償・授業用途でも規約の免除を推測しない。
