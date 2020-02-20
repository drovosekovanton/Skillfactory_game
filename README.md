# Skillfactory_game

Репозиторий является рабочими файлами задания на самостоятельную работу в рамках учёбы на курсе "Python для работы" (платформа Skillfactory).

Задание представляет собой вариант проведения аналитических работ по конкретному датасету.

Получившийся ноутбук документирован, текст исследования и соответствующий код расположены вместе.

#### Исходные файлы:
Предоставлен датасет с kaggle.com:
[Smart meters in London](https://www.kaggle.com/jeanmidev/smart-meters-in-london "Smart meters in London")

#### Требуется:
Выбрать из предложенного для работы датасета те файлы, которые планируется анализировать, извлечь из них нужную информацию и предоставить её в виде отчёта о факторах, влияющих на уровень потребления электрической энергии.

#### Файлы репозитория:
[Skillfactory_game.ipynb](https://github.com/drovosekovanton/Skillfactory_game/blob/master/Skillfactory_game.ipynb "Skillfactory_game.ipynb") - ноутбук для [Google Colab](https://colab.research.google.com/ "Google Colab")

[Relations diagram.pdf](https://github.com/drovosekovanton/Skillfactory_game/blob/master/Relations%20diagram.pdf "Relations diagram.pdf") - схема взаимосвязей отдельных файлов датасета ([оригинал файла](https://drive.google.com/file/d/1YRiAUd_m_7IG9lklkeAsdHPuWDpw_B6P/view "оригинал файла"))

Skillfactory_report - печатная версия ноутбука ([pdf](https://github.com/drovosekovanton/Skillfactory_game/blob/master/Skillfactory_report.pdf "pdf")|[html](https://github.com/drovosekovanton/Skillfactory_game/blob/master/Skillfactory_report.html "html"))

#### Актуальный набор данных для работы
В процессе работы датасет дополнялся и изменялся, актуальная копия датасета лежит на Google Drive:
[Actual dataset](https://drive.google.com/drive/folders/1oVN31sW5rC_RDhA4w3azI0LwELBO3mx5?usp=sharing "Actual dataset")
Изменения:
- файлы из halfhourly_dataset были запакованы в zip-архивы для уменьшения места на диске и увеличения скорости работы с ними
- вручную очищен uk_bank_holidays.csv, убрана лишняя текстовая информация о переносе праздников и произведена корректировка неверного отображения апострофов
- файлы из папки halfhourly_dataset были преобразованы к часовым отсчётам (суммированием потреблённой энергии по каждому счётчику), и положены в папку hourly_dataset. Названия файлов сохранены без изменения
- добавлен файл hourly_energy_use.csv с суммарным почасовым потреблением электроэнергии всеми домохозяйствами
- добавлены файлы std_hour_energy.csv и tou_hour_energy.csv с почасовыми средними значениями потребления электроэнергии всех домохозяйств с соответствующим типом учёта потребления (стандарт или повременной)

Все обновлённые данные (кроме uk_bank_holidays) можно получить, раскомментировав и запустив соответствующий код из ноутбука
