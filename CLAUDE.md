# CLAUDE.md

本 repo 為 LiquidGlassHeaderTemplate 產品的頂層 **Product git**。本產品為 React Native 模板庫，展示 iOS 26 Liquid Glass 風格的原生 Header 實作。

## 四層 git 結構

- **頂層 Product git：**
    - 即本 repo
    - 目前 `no1_product_initiation/`、`no2_product_planning/`、`no5_project_management/` 皆為 placeholder
    - 模板庫本質不需要完整決策框架上游產出，保留結構以備日後擴充
- **Module Design git：**
    - `no3_product_designs/` 容器目錄已預留，目前無 Design git
    - 模板庫的視覺由 Impl 直接承載
- **Module Spec git：**
    - `no4_product_specs/no1_liquid_glass_header/`
    - 空殼 git，待需要時補 Model / View / Logic 三層規格
- **Module Impl git：**
    - `no6_product_development/no1_liquid_glass_header/`
    - React Native template 本體

## 當前 module 註冊

- `no1_liquid_glass_header`
    - Design git：尚無
    - Spec git：`no4_product_specs/no1_liquid_glass_header/`（空殼）
    - Impl git：`no6_product_development/no1_liquid_glass_header/`

---

## 歷史

本 repo 由原 `LiquidGlassHeaderTemplate/` 單層 git 重構而來。原 git 搬到 `no6_product_development/no1_liquid_glass_header/` 作為 Module Impl git，頂層新建 Product git 承載產品元資訊。

2026-05-15 配合四層 git 重構，將原 `no3_product_specs/` 重編為 `no4_product_specs/`、`no4_project_management/` 重編為 `no5_project_management/`、`no5_product_development/` 重編為 `no6_product_development/`，新增 `no3_product_designs/` 容器目錄。

---

## 撰寫規範

任何改動前先 consult `decision_framework_router` skill 的上游 review 四問。模板庫的改動多屬純 Impl 範疇，auditor 會得 `REFACTOR_EXEMPT` 或 `IMPL_ONLY`（Spec git 空殼）。若 API 或使用說明有變動，需同步更新 Spec git。
