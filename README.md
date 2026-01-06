# USA Auto Hub Mapper

米国内の自動車関連製造拠点を可視化・管理するインタラクティブなマップアプリケーション。
完成車メーカー（OEM）と部品メーカー（Tier1サプライヤー）の58拠点を網羅。

## 機能

### マップビュー
- **ホバーツールチップ**: 拠点ポイントにマウスを近づけると、詳細情報が表示されます
  - メーカー名
  - 所在地（都市、州）
  - 製品タイプ
  - 生産能力
  - 詳細情報
  - 地域バッジ（日系/米国系/欧州系/韓国系/その他）
  - 業態バッジ（完成車メーカー/部品メーカー）
- **クリックポップアップ**: マーカーをクリックすると、より詳細な情報がポップアップで表示されます

### フィルタリング機能
- **業態フィルター**: 完成車メーカー(OEM)、部品メーカー(Tier1)
- **地域フィルター**: 日系、米国系、欧州系、韓国系、その他
- **工程フィルター**:
  - 完成車組立
  - プレス/成形
  - パワートレイン
  - 電子部品
  - 内装
  - 外装
  - シャーシ
  - シート
  - バッテリー
  - タイヤ/ゴム
  - ガラス
- **検索**: メーカー名、州、都市、製品タイプ、工程で検索

### テーブルビュー
- ソート機能付きのデータテーブル
- 行をクリックしてマップ上の拠点にジャンプ

### 統計ダッシュボード
- 総拠点数
- 日系メーカー数
- 米国系メーカー数
- 欧州系メーカー数
- アジアその他メーカー数
- 部品メーカー数

### エクスポート
- CSV形式でデータをエクスポート可能

## 技術スタック

- **Leaflet**: 地図表示
- **Tailwind CSS**: スタイリング
- **Lucide Icons**: アイコン

## データ構成

### 拠点数: 58箇所

#### 完成車メーカー (OEM) - 22拠点

**日系OEM (7拠点)**
- Toyota Motor Manufacturing Kentucky (Camry, RAV4 Hybrid)
- Honda Development & Mfg of America (Accord, CR-V)
- Nissan North America Smyrna Plant (Leaf, Rogue)
- Toyota Motor Manufacturing Texas (Tundra, Sequoia)
- Subaru of Indiana Automotive (Outback, Legacy)
- Mazda Toyota Manufacturing USA (CX-50, CX-70)
- Mitsubishi Motors North America (Outlander)

**米国系OEM (4拠点)**
- GM Factory ZERO (Hummer EV, Silverado EV)
- Ford Rouge Electric Vehicle Center (F-150 Lightning)
- Ford Kentucky Truck Plant (F-150, Expedition)
- Stellantis Jeep Assembly (Jeep Grand Cherokee)

**欧州系OEM (4拠点)**
- BMW Plant Spartanburg (X3, X4, X5, X6, X7)
- Mercedes-Benz Tuscaloosa (GLE, GLS)
- Volkswagen Chattanooga (ID.4, Atlas)
- Volvo Cars Ridgeville (S60, EX90)

**韓国系OEM (3拠点)**
- Hyundai Motor Manufacturing Alabama (Elantra, Santa Fe)
- Kia Motors Manufacturing Georgia (Telluride, Sorento)
- Hyundai Motor Group Metaplant America (IONIQ 5, EV9)

**その他EVメーカー (4拠点)**
- Tesla Giga Texas (Model Y, Cybertruck)
- Tesla Factory Fremont (Model 3, S, X, Y)
- Rivian Normal Plant (R1T, R1S)
- Lucid Motors Casa Grande (Lucid Air)

#### 部品メーカー (Tier1) - 36拠点

**バッテリーメーカー (5拠点)**
- LG Energy Solution Michigan
- Panasonic Energy Kansas
- BlueOval SK Battery Park
- SK On Battery Georgia
- Samsung SDI Michigan

**日系部品メーカー (13拠点)**
- DENSO Manufacturing Tennessee (スターター、オルタネーター、ECU)
- Aisin Manufacturing Kentucky (自動変速機、ドアモジュール)
- JTEKT Manufacturing North Carolina (ステアリング、ドライブシャフト)
- Calsonic Kansei North America (HVAC、ラジエーター)
- Yokohama Tire Virginia (乗用車タイヤ)
- Bridgestone Americas Tennessee (乗用車・トラックタイヤ)
- Sumitomo Electric West Virginia (ワイヤーハーネス)
- NSK America Indiana (ベアリング)
- Toyota Boshoku Alabama (シート、インテリアトリム)
- Koito Manufacturing Virginia (ヘッドランプ、テールランプ)
- NSG Pilkington Ohio (自動車ガラス)
- Toyota Gosei Kentucky (ゴムシール、ホース)
- Alps Alpine Michigan (電子機器、ナビゲーション)

**米国系部品メーカー (5拠点)**
- Magna International Tennessee (シート、フレーム)
- Dana Incorporated Kentucky (プロペラシャフト)
- BorgWarner Michigan (ターボチャージャー、トランスミッション)
- Visteon Michigan (電子機器、クラスター)
- American Axle Michigan (ドライブシャフト)

**欧州系部品メーカー (7拠点)**
- Continental AG South Carolina (タイヤ、ブレーキシステム)
- ZF Group North Carolina (トランスミッション)
- Bosch South Carolina (燃料噴射システム、センサー)
- Valeo South Carolina (スターター、オルタネーター)
- Michelin South Carolina (乗用車タイヤ)
- Faurecia Michigan (シート、インテリア)
- Valeo Tennessee (冷却システム)

**韓国系部品メーカー (4拠点)**
- Hyundai Mobis Alabama (モジュール、コンポーネント)
- Hyundai Mobis Georgia (バンパー、ラジエーター)
- Hankook Tire Tennessee (乗用車タイヤ)
- Kumho Tire Georgia (乗用車タイヤ)

**その他部品メーカー (2拠点)**
- Goodyear Tire & Rubber Ohio (乗用車・トラックタイヤ)
- Cooper Tire Mississippi (乗用車タイヤ)

## カテゴリー体系

### 地域別
- **日系**: 日本企業の拠点
- **米国系**: アメリカ企業の拠点
- **欧州系**: ヨーロッパ企業の拠点
- **韓国系**: 韓国企業の拠点
- **その他**: Tesla、Rivian等の新興EVメーカー

### 業態別
- **完成車メーカー(OEM)**: 自動車の完成車を製造するメーカー
- **部品メーカー(Tier1)**: 完成車メーカーへ直接部品を納入するサプライヤー

### 製品タイプ
- **完成車組立**: 乗用車、トラック等の完成車の組立
- **プレス/成形**: 金属プレス、樹脂成形
- **パワートレイン**: エンジン、変速機、駆動システム
- **電子部品**: ECU、センサー、ハーネス等
- **内装**: シート、インテリアトリム、HVAC
- **外装**: バンパー、ランプ、ガラス
- **シャーシ**: サスペンション、ステアリング、ブレーキ
- **シート**: シート専用工場
- **バッテリー**: EV用バッテリーセル
- **タイヤ/ゴム**: タイヤ、ゴム部品
- **ガラス**: 自動車ガラス

## 更新履歴

### 2025-01-06 (v2.0)
- パーツメーカー（Tier1サプライヤー）36拠点を追加
- データ構造を拡張（origin、type、processLabel等）
- 地域別カテゴリーを追加（日系/米国系/欧州系/韓国系/その他）
- 業態別カテゴリーを追加（完成車メーカー/部品メーカー）
- 製品タイプを詳細化（11種類の工程タイプ）
- 統計ダッシュボードを拡張（6つの統計項目）
- フィルター機能を強化（業態、地域、工程の3つでフィルタリング可能）
- ホバーツールチップ機能の追加

### 2025-01-06 (v1.0)
- 初版リリース
- 完成車メーカー15拠点のマッピング
- 基本的なフィルタリングと検索機能

## ライセンス

&copy; 2025 Auto Map System. All Rights Reserved.
