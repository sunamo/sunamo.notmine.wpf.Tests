# sunamo.notmine.wpf.Tests

Testovací WPF aplikace (`TestUI`, .NET 9) pro ruční vyzkoušení ovládacího prvku `SearchTextBox`.

## Obsah

- `SearchTextBox.Tests` – WPF projekt s oknem `Window1`.
- Okno obsahuje `SearchTextBox`, seznam `ListBox` s položkami `ab`, `ac`, `bb`, `bc` a pole pro obsah hledání.
- Kód nastavuje styl sekcí (`RadioBoxStyle`) a obsluhuje událost `OnSearch`.

## Poznámky

- Projekt se odkazuje na `..\..\..\sunamo.notmine\SearchTextBox\SearchTextBox.csproj`, který v repu není.
- Bez toho projektu se aplikace nezbuilduje.
- Řešení: `sunamo.notmine.wpf.Tests.sln`.
