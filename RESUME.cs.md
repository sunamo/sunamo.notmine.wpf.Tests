---
schema_version: 11
type: tests
category_override: none
file_count: 14
file_extensions: cs:5, md:2, xaml:2, csproj:1, jsonanddelete:1, noext:1, resx:1, settings:1, slnx:1
file_extensions_updated: 2026-10-04
avg_lines_per_file: 28
total_lines: not run
metrics_lm: 2026-10-01 16:41:13
move_to_legacy_percent: 90
description_updated: 2026-10-01
links_updated: 2026-10-01
github_source_url: not found
origin_status: found
origin_checked: 2026-10-01
article_source_url: not run
article_status: pending
article_checked: not run
last_build_ok: not run
last_build_date: not run
last_tests_run_date: not run
covered_lines: not run
---

## Description

Testovací WPF aplikace `TestUI` (.NET 9), která v jednom okně ukazuje ovládací prvek `SearchTextBox` s filtrováním jednoduchého seznamu. Repo neobsahuje samotný ovladač, jen ProjectReference na `sunamo.notmine\SearchTextBox`, takže se samo nezbuilduje. Jde o ukázkové okno bez produkčního využití.

## Původ zdrojáků

Staženo z GitHubu: **ne** — nenalezen žádný zdroj na GitHubu, kód vznikl v repech sunamo.
- Ověřeno: origin `sunamo/sunamo.notmine.wpf.Tests`, historie od 2023-11 jen autoři sunamo, žádné URL ani copyright v kódu. `gh search repos` "SearchTextBox WPF sections radio" a `gh search code` "ShowSectionButton SectionsStyles", "m_txtTest_OnSearch SearchEventArgs" nevrátily žádnou shodu, hash kandidáta tedy nebyl s čím porovnat. Testovaný ovladač je pravděpodobně z internetu (viz `SearchTextBox_JustDecompile` v `E:\vs_FromNetButNotOnPackageManager`), ale to není doložené GitHub repo.

## Doporučení přesunu do legacy

Doporučení přesunu do sunamocz-legacy.visualstudio.com: **90 %** — jen ruční testovací okno pro ovladač, který v repu není.
- Projekt nejde zbuildit, protože chybí odkazovaný `SearchTextBox.csproj`.
- Žádná logika ani testy, jen `Window1` s pár položkami.
- Poslední commit z 2024-12, ovladač se drží jinde.

## Vazby na moje repa

- Submoduly: žádné
- ProjectReference / PackageReference: `SearchTextBox` (ProjectReference, cíl chybí)
