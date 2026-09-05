# docx-automation-examples — демонстрационные документы формата docx-automation-spec

> Часть набора [docx-automation](https://github.com/Artem891372/docx-automation):
> [spec](https://github.com/Artem891372/docx-automation-spec) ·
> [validator](https://github.com/Artem891372/docx-automation-validator) ·
> [examples](https://github.com/Artem891372/docx-automation-examples)

Анонимизированные примеры документов для формата
[docx-automation-spec](https://github.com/Artem891372/docx-automation-spec). Каждый YAML-файл — самостоятельный документ,
который можно собрать в DOCX движком, поддерживающим спецификацию, и который
проходит проверку [валидатором](https://github.com/Artem891372/docx-automation-validator):

```bash
# если репозиторий validator склонирован рядом
python3 ../docx-automation-validator/validate_document.py kursovaya_banking_app.yml
```

## Что внутри

| Файл | Что демонстрирует |
|---|---|
| [`kursovaya_banking_app.yml`](kursovaya_banking_app.yml) | Курсовая про классификацию обращений в техподдержку мобильного банка (ML). Диаграммы PlantUML и графики Matplotlib встроены прямо в YAML (`diagram_type: kroki` / `matplotlib`), скриншоты приложения — в `screenshots/`. Показывает: формулы LaTeX, таблицы с данными экспериментов, листинги кода, перекрёстные ссылки `{ref:...}`, список источников |
| [`kursovaya_lan_store.yml`](kursovaya_lan_store.yml) | Курсовая по компьютерным сетям: проект ЛВС магазина. Показывает: растровые схемы (`path: images/...`), приложения с буквенной нумерацией, кабельный журнал, таблицы оборудования |
| [`mini_methodology_guide.yml`](mini_methodology_guide.yml) | Короткий методический документ (требования к курсовой работе). Показывает: бланки титульных листов, простые таблицы, структуру «методички» |

Папки `images/` и `screenshots/` содержат иллюстрации, на которые ссылаются
примеры (`path` указывается относительно каталога с YAML-файлом).

## Про анонимизацию

Примеры получены из реальных студенческих работ и **обезличены**:

- названия компаний-предметов заменены вымышленными («Альфа-Маркет», ООО «Альфа»),
- адреса и города заменены («г. Энск, ул. Центральная, 1»),
- ФИО преподавателей и руководителей заменены,
- упоминания конкретного вуза и кафедры удалены.

Ссылки на публичные источники (книги, ГОСТ, статьи) сохранены как есть.

## Лицензия

MIT — см. [LICENSE](LICENSE).
