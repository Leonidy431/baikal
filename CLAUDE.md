# CLAUDE.md — baikal

## Linux на Android: Terminal и Termux (2026-11-26)
- **Terminal** — приложение Android (AVF), не функция GrapheneOS; есть и на обычном Pixel. Это Debian в виртуальной машине; образ (от ~500 МБ) качается с серверов Google. На Pixel 10 — почти нативная скорость и GPU-ускорение, но графика с серьёзными ограничениями. В GrapheneOS пакет `com.android.virtualization.terminal`, поведение то же.
- **Включение (по памяти оператора, источниками не подтверждено):** режим разработчика → Настройки → Система → Параметры разработчика → «Среда разработки Linux». Внутри: `apt install nodejs npm git`, затем `npx skills …`.
- **Termux** — нативный userland, минимальные накладные расходы, F-Droid/GitHub, файлы через `termux-setup-storage` (в Terminal — `/mnt/shared`). Для `npx skills` годятся оба; для быстрого старта — Termux.
- Полная справка и план для VM8: `Leonidy431/webtypicon2` → `docs/version-3.0/HLD/docs/ru/HLD_ДЕКЕЙ_VM8_ИНСТРУМЕНТЫ_NODE_SKILLS_2026-11-26.md`. Источники: reddit.com/r/Android/comments/1obt3vf · android.gadgethacks.com (Pixel 10 GPU acceleration) · discuss.grapheneos.org/d/30425 · discuss.grapheneos.org/d/42966 · github.com/termux/termux-app/releases
