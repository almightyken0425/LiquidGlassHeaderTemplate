# LiquidGlassHeaderTemplate 產品規則

- 本 repo 是產品的 Product git
- 產品是 React Native 模板庫
- 目標為 iOS Liquid Glass Header

## 多層 git 結構

- Product git 保留提案與規劃層
- 上游內容目前是 placeholder
- Spec git 是已註冊空殼
- Design git 尚未建立
- Impl git 承載模板本體
- Module 配對以 `decision_framework_router` 的註冊表為準

---

## Module 註冊

- module id 為 `no1_liquid_glass_header`
- Spec git 位於 `no3_product_specs/no1_liquid_glass_header/`
- Impl git 位於 `no5_product_development/no1_liquid_glass_header/`
- 視覺目前由 Impl 直接承載

---

## 原生工作規則

- 任何改動先使用 `decision_framework_router`
- Markdown 改動使用 `universal_writing_linter`
- Spec 文件改動先使用 `spec_writer`
- Header 實作改動使用 `rn-native-header`
- 純內部重構可維持 Impl 單層
- 對外 API 變動要同步 Spec
- 元件行為變動要同步 Spec
- 跨層 branch 名稱必須一致
- 配對 commit 內容必須一致

---

## 歷史脈絡

- 原單層 git 已成為 Module Impl git
- Product git 承載產品元資訊
- 專案管理已移至工作區根層
- 現行層編號自 2026-07-21 生效

---

## 相容與漂移控制

- `AGENTS.md` 是本目錄的規則真相
- `CLAUDE.md` 只保留 Claude Code 入口
- 產品規則不得複製回相容入口
- 漂移檢查確認相容入口只含導向規則
