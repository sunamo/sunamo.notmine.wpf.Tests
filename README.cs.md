# sunamo.notmine.wpf.Tests

## Short description

Testovací WPF aplikace `TestUI` (.NET 9), která v jednom okně ukazuje ovládací prvek `SearchTextBox` s filtrováním jednoduchého seznamu. Repo neobsahuje samotný ovladač, jen ProjectReference na `sunamo.notmine\SearchTextBox`, takže se samo nezbuilduje. Jde o ukázkové okno bez produkčního využití.

Testovací WPF aplikace (`TestUI`, .NET 9) pro ruční vyzkoušení ovládacího prvku `SearchTextBox`.

## Obsah

- `SearchTextBox.Tests` – WPF projekt s oknem `Window1`.
- Okno obsahuje `SearchTextBox`, seznam `ListBox` s položkami `ab`, `ac`, `bb`, `bc` a pole pro obsah hledání.
- Kód nastavuje styl sekcí (`RadioBoxStyle`) a obsluhuje událost `OnSearch`.

## Poznámky

- Projekt se odkazuje na `..\..\..\sunamo.notmine\SearchTextBox\SearchTextBox.csproj`, který v repu není.
- Bez toho projektu se aplikace nezbuilduje.
- Řešení: `sunamo.notmine.wpf.Tests.slnx`.
