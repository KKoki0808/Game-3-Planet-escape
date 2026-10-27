> Publication scope update (2026-10-27): This file is part of a documentation-only publication. References below to pending publication concern the full Unity project, media and Windows game, or earlier preparation steps. See [PUBLICATION_STATUS.md](PUBLICATION_STATUS.md) for current scope. No underlying media is included.

# Planet Escape 素材の権利・提出方法レビュー

確認日：2026-10-26。公開操作は行っていません。今回の判断は現在取得できる公式規約とローカル記録に基づきます。生成日時ごとの規約同意履歴・個別許諾書を取得したものではありません。

## 出典の分類（31素材）

ユーザーは「自分で作りました」「両方とも無料」と回答しました。21モデルと8効果音は、本人生成・生成当時無料プランとして記録します。これは本人申告の確認であり、生成履歴画面を独立監査した意味ではありません。Taratect_Colorを含む4つのZIPも同じ扱いとし、従来の「生成者不明」を現在の結論として残しません。

| 分類 | 件数 | 根拠 |
| --- | ---: | --- |
| 1. 自分で生成 | 30 | Tripoモデル21、ElevenLabs効果音8、別サービスOpenAIによる記録済み生成空画像1 |
| 2. 他人が生成・公開 | 0 | 該当すると確認された素材なし |
| 3. Unity／外部アセットストア取得 | 0 | この31素材内では該当確認なし |
| 4. 出典不明 | 1 | 星空の参考写真。実行時の空画像とは別。公開対象から除外済み |

Unity Package Managerの依存パッケージは、この31素材とは別集計です。[パッケージ別ライセンス一覧](THIRD_PARTY_NOTICES.md)と保存済み原文を参照してください。Asset Storeモデルと混同しません。

## 利用形態ごとの判定

「条件付き可」は一般的な利用許可の確認であり、全入力の権利まで監査済みという意味ではありません。「要確認」は禁止の断定でも、すべての使用権が不明という意味でもありません。授業提出は非商用として扱う想定ですが、無償というだけであらゆる商用目的が消えるわけではありません。

| 規則 | 素材 | ゲーム内使用 | GitHubの素材ソース公開 | Windowsゲームへの組み込み配布 |
| --- | --- | --- | --- | --- |
| T | Tripo Free 21件 | 非商用利用の一般許可を確認 | 無料出力の再配布・再許諾範囲は要確認 | 非商用組み込みは利用許可と整合する解釈。ただし無料出力配布の明確な範囲を確認してから公開 |
| E | ElevenLabs Free 8件 | 非商用・指定クレジット等を満たせば可 | MP3単体配布は制限対象。通常のGitHub公開は許諾済みにできない | 他の素材と組み合わせたゲームは条件付き可。非商用・指定クレジット等が必要 |
| O | OpenAI生成の空1件 | 出力権利は裏付けあり。参考入力の権利は別問題 | 同左 | 同左 |
| R | 出典不明の参考写真1件 | 実行時には不使用 | 除外を維持 | 実行時には不使用。追加しない |

### T：Tripo

[料金ページ](https://www.tripo3d.ai/pricing)はFreeを非商用利用と明示します。[規約](https://www.tripo3d.ai/terms)（2025-07-11更新）3.2は適法な出力利用を認め、第三者提供が契約と整合することを要求します。5.2.1は無料ユーザーの出力等に関する権利をTripo側に留保しています。従って「自作だから全権利を保有」「非商用利用も一切不明」のどちらも採用しません。無料モデルのGLB/FBX・変換メッシュ等を第三者へ再配布する具体的範囲は明確に確定できず、組み込みゲームについても限定した照会が適切です。未確認のCCライセンスを割り当てません。今から有料化して過去素材に遡及するとは扱いません。

### E：ElevenLabs

[公式公開ガイド](https://elevenlabs.io/docs/help-center/legal/can-i-publish-the-content-i-generate-on-the-platform)は無料生成物を非商用に限定し、公開時のタイトルに `elevenlabs.io` または `11.ai` を含めるよう要求します。[ElevenCreative Terms](https://elevenlabs.io/creative-terms)（2026-10-09更新）Exhibit 4 §2はゲーム等への組み込みを認める一方、孤立した音声ファイル・サンプル等の提供を制限します。公式Community Sharing等の例外は、一般のGitHubへのアップロードとは別です。必要なのは8音の作り直しではなく、組み込み利用の条件遵守とMP3単体公開の分離です。有料化だけで単体音声制限がなくなるとは解釈しません。Betaで生成した場合は追加条件も適用されます。

### O：生成した空と参考写真

[OpenAI Terms of Use](https://openai.com/policies/terms-of-use/)（2026-01-01発効、Content）およびAPI等に該当する場合の[Services Agreement](https://openai.com/policies/services-agreement/)を参照。サービスとの関係での出力権利は利用者に帰属する構造ですが、第三者の権利・入力許諾まで付与しません。空画像の生成記録は `Assets/PlanetEscape/Art/SkyJet/MilkyWayPanorama.prompt.md` にあります。参考写真はスタイル参考であり、写真自体の配布許諾は未記録です。参考を使ったというだけで生成出力の侵害を断定しませんが、入力の権利根拠は別途残る確認事項です。

### 分類2・3についての一般則（今回の素材には該当確認なし）

他人の公開物は、公開されているだけでは再配布許可になりません。作品ごとのライセンス・生成者の許諾を確認します。[Unity Asset Store EULA](https://unity.com/legal/as-terms)2.2.1は条件を満たすゲームへの組み込み配布を認めますが、通常、素材そのものを公開リポジトリで配布する許可とは異なります。Restricted Assetや独自規約は個別確認が必要です。外部ストアにも一律の共通許諾はありません。

## 31素材の個別一覧

次の記号は上記規則の3用途別判定に対応します。元ファイル名・SHA256・確認事項・公式参照URLは[CSV](ASSET_LICENSE_INVENTORY.csv)に保存しています。派生したメッシュ、テクスチャ、FBX、音声にも元素材の条件を引き継いで検討します。

| ID | 元素材 | 分類 | 規則 | プロジェクト内パス |
| --- | --- | --- | --- | --- |
| A01 | alien+egg+cluster+3d+model.glb | 1 | T | `Assets/PlanetEscape/AlienNest/Art/Egg/Source.glb` |
| A02 | futuristic+gun+3d+model.glb | 1 | T | `Assets/PlanetEscape/AlienNest/Art/Gun/Source.glb` |
| A03 | spacecraft+module+3d+model.glb | 1 | T | `Assets/PlanetEscape/AlienNest/Art/SpacecraftModule/Source.glb` |
| A04 | spider+web+3d+model.glb | 1 | T | `Assets/PlanetEscape/AlienNest/Art/Web/Source.glb` |
| A05 | 宇宙飛行士スーツ3dモデル.glb | 1 | T | `Assets/PlanetEscape/Art/Astronaut/Source/AstronautOriginal.glb` |
| A06 | 宇宙飞船3d模型.glb | 1 | T | `Assets/PlanetEscape/Art/CrashedShip/Source/SpacecraftOriginal.glb` |
| A07 | gpu+chip+3d+model.glb | 1 | T | `Assets/PlanetEscape/Art/NavigationChip/Source/Original.glb` |
| A08 | 岩石墙+3d+模型.glb | 1 | T | `Assets/PlanetEscape/Art/RockyCanyon/Cliff/Source/Original.glb` |
| A09 | 岩石3d模型.glb | 1 | T | `Assets/PlanetEscape/Art/RockyCanyon/Stone/Source/Original.glb` |
| A10 | surveillance+camera+3d+model.glb | 1 | T | `Assets/PlanetEscape/DroneBase/Art/Camera/Source.glb` |
| A11 | industrial+cargo+crate+3d+model.glb | 1 | T | `Assets/PlanetEscape/DroneBase/Art/Crate/Source.glb` |
| A12 | rocket+engine+3d+model.glb | 1 | T | `Assets/PlanetEscape/DroneBase/Art/Engine/Source.glb` |
| A13 | futuristic+container+3d+model.glb | 1 | T | `Assets/PlanetEscape/DroneBase/Art/FutureContainer/Source.glb` |
| A14 | military+truck+3d+model.glb | 1 | T | `Assets/PlanetEscape/DroneBase/Art/MilitaryTruck/Source.glb` |
| A15 | shipping+container+3d+model.glb | 1 | T | `Assets/PlanetEscape/DroneBase/Art/Shipping/Source.glb` |
| A16 | mobile+laboratory+truck+3d+model.glb | 1 | T | `Assets/PlanetEscape/DroneBase/Art/Truck/Source.glb` |
| A17 | industrial+cargo+crate+3d+model (1).glb | 1 | T | `Assets/PlanetEscape/DroneBase/Art/WallCrate/Source.glb` |
| A18 | rock+stack+3d+model+ghibli+style.zip | 1 | T | `Assets/PlanetEscape/AlienNest/Art/Rock/Source.zip` |
| A19 | Taratect_Color.fbx.zip | 1 | T | `Assets/PlanetEscape/AlienNest/Art/Spider/Source.zip` |
| A20 | 浮遊防衛ドローン3dモデル.zip | 1 | T | `Assets/PlanetEscape/DroneBase/Art/Drone/Source.zip` |
| A21 | tank+container+3d+model.zip | 1 | T | `Assets/PlanetEscape/DroneBase/Art/Tank/Source.zip` |
| A22 | A_futuristic_securit_#2-1793063117195.mp3 | 1 | E | `Assets/PlanetEscape/Audio/Experience/DroneSecurity.mp3` |
| A23 | A_very_short,_sharp__#2-1793053057518.mp3 | 1 | E | `Assets/PlanetEscape/Audio/Experience/RifleSharp.mp3` |
| A24 | The_sound_of_electro_#2-1793057219449.mp3 | 1 | E | `Assets/PlanetEscape/Audio/Experience/ShipElectrical.mp3` |
| A25 | A_futuristic_spacesh_#4-1793062733368.mp3 | 1 | E | `Assets/PlanetEscape/Audio/Experience/ShipStartup.mp3` |
| A26 | A_terrifying_alien_s_#1-1793053087913.mp3 | 1 | E | `Assets/PlanetEscape/Audio/Experience/SpiderAlien.mp3` |
| A27 | A_very_short,_sharp__#2-1792934648647.mp3 | 1 | E | `Assets/PlanetEscape/Resources/PlanetEscapeAudio/JetJump.mp3` |
| A28 | A_short,_satisfying__#4-1792934973953.mp3 | 1 | E | `Assets/PlanetEscape/Resources/PlanetEscapeAudio/PartPickup.mp3` |
| A29 | 宇宙船飛び立つ音.mp3 | 1 | E | `Assets/PlanetEscape/Resources/PlanetEscapeAudio/ShipLaunch.mp3` |
| A30 | MilkyWayPanorama-v1.png | 1 | O | `Assets/PlanetEscape/Art/SkyJet/MilkyWayPanorama-v1.png` |
| A31 | MilkyWay-reference.jpg | 4 | R | `Assets/PlanetEscape/Art/SkyJet/Reference/MilkyWay-reference.jpg` |

## 最小限の追加作業で提出する案

1. **ゲームとZIPはそのまま保管**。Tripoへ「本人が無料プランで生成したモデルを、非商用のAME294授業用Windowsゲームに組み込み、無料配布できるか。モデル単体は配布しない」と一括照会する。原本公開も必要なら、GLB/FBXと変換メッシュ・テクスチャの公開範囲を同じ照会で分けて確認する。21件を他人の素材として再調査する必要はない。
2. **ElevenLabsは生MP3を公開しない案を優先**。公開タイトル案は `Planet Escape — SFX by ElevenLabs (11.ai)`。Release本文・READMEにも出典を記載する。既存バイナリを変えず外側のReleaseタイトルで指定条件を満たせるかは公式ガイドだけでは確定できないため、その点だけ確認する。必要なら担当教員にも提出形態を確認する。教員への限定共有も権利条件の自動免除ではない。
3. **参考写真は公開しない**。本人撮影・利用許諾・その他の入力利用根拠があるかだけ確認する。空を作り直すことは今回行わない。
4. **ソースはコード・説明資料に限定した別の公開用スナップショットを提案**。現在のローカル履歴にはMP3等が既に含まれるため、今のmainをそのままPushせず、元履歴を保存したまま独立した公開用履歴を用意する方法がある。`.gitignore`への後付けだけでは過去コミットの素材を隠せない。モデル原本だけでなく派生メッシュ・テクスチャ・音声も公開対象から外す。この案は完全再構築可能なUnityプロジェクトではない。課題が完全ソース必須なら、該当素材の再配布許諾か提出方法の合意が必要。
5. 上記の配布条件が解決したら、既存ZIPを変更せずReleaseへ登録し、正しいダウンロードリンクを記載する。未解決のままReleaseを公開しない。

今回実施したのは一覧・判定・提出案の更新のみです。サポートへの送信、Push、Release作成、アップロード、履歴変更、ゲームやビルドの変更は行っていません。許諾不明の素材をコードだけの公開案に紛れ込ませることも認めていません。


## 2026-10-27 publication preparation update

The author confirmed this is a noncommercial university assignment. Rechecked Tripo terms/pricing/help and ElevenLabs Sound Effects/publishing guidance; the distinction between Free noncommercial use, source media redistribution and embedded-game publication remains. See [the final submission plan](SUBMISSION_PUBLICATION_PLAN.md), [file-level held-file ledger](PUBLICATION_FILE_DECISIONS.csv), [unsent inquiries](LICENSE_INQUIRIES.md) and [conditional Release draft](RELEASE_DRAFT.md). README title and explicit ElevenLabs credits are now prepared; attribution placement compliance is not assumed. No asset or binary was changed or uploaded.
