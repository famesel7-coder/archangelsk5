# Approved Assets — «Архангельск 5»

Эта папка содержит утверждённые пользователем исходные SVG проекта. Использовать файлы напрямую; не реконструировать их по памяти и не заменять похожими иллюстрациями.

## Asset manifest

| Asset | Repository path | Source filename | Canvas | SHA-256 |
|---|---|---|---:|---|
| Белый знак «Пятёрочки» | `brand/pyaterochka-5-mark-white.svg` | `Group 2131329780.svg` | 57 × 57 | `1568b6ce90bd08c6a541cc5c957b07ce6513d11b1328b1f1e06c6e78fe69b091` |
| Ледокол «Диксон» | `illustrations/ship-dikson.svg` | `Корабль.svg` | 1059 × 836 | `038f6a0940bab8ed2fff89be0b63a2131642d26447be0e2e972631ed26398c21` |
| Маяк | `illustrations/lighthouse.svg` | `Маяк.svg` | 178 × 797 | `85c300917247676f56fe5f91e08bf84145a1c3f19c724dd3ccad816381b13caf` |
| Пётр I | `illustrations/peter-i.svg` | `Петр I.svg` | 437 × 848 | `1460dfb693f1e2bddc5e71cacb818ac74c04797e76d51ad7aac36aefb7425f29` |

Все файлы — чистые vector SVG без embedded image, text или script elements.

## Logo policy

`brand/pyaterochka-5-mark-white.svg` — critical logo asset: белая фирменная «5» с листом внутри белой окружности.

- использовать точный SVG;
- сохранять aspect ratio и path geometry;
- не заменять цифрой 5, текстом, похожей иконкой или AI-generated знаком;
- не mirror, rotate, distort или recolor без утверждённого варианта;
- не использовать как повторяющийся декоративный pattern;
- cover, section/brand statement и closing-слайды с явным отправителем «Пятёрочка» должны содержать знак, если он уже не обеспечен master-layout;
- minimum size, safe area и фиксированный placement пока не подтверждены — брать из утверждённого master/Figma-макета.

## Illustration policy

Для `ship-dikson.svg`, `lighthouse.svg` и `peter-i.svg`:

Разрешено:

- proportional scale;
- translation;
- crop через frame/mask;
- layering с перспективой, типографикой и другими объектами.

Запрещено:

- mirroring;
- distortion и непропорциональный scale;
- path simplification или ручная перерисовка;
- AI-generated/lookalike replacement;
- unapproved recolor;
- изменение внутренних fills `#262424` у корабля.

## Integrity check

После любого переноса или автоматической обработки сравнить SHA-256 с манифестом. Несовпадение означает, что файл изменён и больше не является оригинальным approved source.
