# 熱阻換算器

工程用 PWA，協助在熱傳導係數、厚度、面積熱阻與總熱阻之間快速換算。

## 功能

- k → 面積熱阻 R″
- 面積熱阻 R″ → 等效 k
- 指定面積後換算總熱阻 K/W
- 指定熱量後估算材料溫差
- 多層材料串聯與熱阻占比
- SI／英制常用單位轉換
- DIV-300 與 DM-800A 快速範例
- 可安裝並離線使用

## 主要關係式

R″ = t / k

R = R″ / A

ΔT = Q × R

多層串聯：R″total = Σ(tᵢ / kᵢ)

## Darbond 預設值

| 材料 | 建模厚度 | 等效 k | 對應 TDS 熱阻 |
| --- | ---: | ---: | ---: |
| DIV-300 | 0.20 mm | 6.20 W/m·K | 0.050 °C·in²/W |
| DM-800A | 0.05 mm | 12.92 W/m·K | 0.006 °C·in²/W |

等效 k 用於讓指定厚度的 FloTHERM XT 實體模型重現 TDS 面積熱阻。若採用這組等效值，不應再重複加入相同的接觸熱阻。

## GitHub Pages

到 repository 的 Settings → Pages，將 Source 選為 GitHub Actions。完成後，每次推送 main 都會自動發佈。
