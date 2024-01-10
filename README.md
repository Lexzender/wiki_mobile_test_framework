# Фреймворк для автоматизации тестирования мобильного приложения ["Wikipedia"](https://www.wikipedia.org/)

<img align="center" src="https://github.com/Lexzender/wiki_mobile_test_framework/blob/main/utils/pictures/wiki.png" />

---

## Особенности проекта
* Запуск mobile автотестов в BrowserStack
* Автоматизация отчетности о тестовых прогонах и тест-кейсах в Jira
* Интеграция с Allure TestOps
* Отчеты Allure Report
* Сборка проекта в Jenkins
* Отчеты с видео, скриншотом, логами, исходной моделью разметки страницы
* Оповещения о тестовых прогонах в Telegram
---
## Список проверок, реализованных в проекте
* Проверка экрана приветствия
* Поиск статей
* Проверка сохранения истории поиска
* Проверка добавления статей в избранное

 ---
## Запуск проекта
Запустить проект можно локально по команде

```
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
pytest -s -v --context=${CONTEXT}
```
Или в Jenkins
### Запуск проекта в Jenkins

1) Открыть [проект](https://jenkins.autotests.cloud/job/wiki_mobile_test_framework/)
2) Нажать "Build with Parameters"
3) Заполнить параметры 
4) Нажать "Build"
<img align="center" src="https://github.com/Lexzender/luma_UI_test_framework/blob/main/luma_UI_test_framework/pictures/jenkins.png" />

---

## Allure report
### После прохождения тестов результаты можно посмотреть в Allure отчете
<img align="center" src="https://github.com/Lexzender/wiki_mobile_test_framework/blob/main/utils/pictures/allure_mob.png" />

### В отчете для каждого теста указана мета информация, а также приложены результаты прохождения: видео, html страницы, скриншот после прохождения.
<img align="center" src="https://github.com/Lexzender/wiki_mobile_test_framework/blob/main/utils/pictures/allure_video_mob.png" />

### Пример прохождения mobile-теста
<img align="center" src="https://github.com/Lexzender/wiki_mobile_test_framework/blob/main/utils/pictures/test_dave_article.gif" />


---
## Нотификация в Telegram
После прохождения тестов результаты будут отправлены в Telegram
<img align="center" src="https://github.com/Lexzender/luma_UI_test_framework/blob/main/luma_UI_test_framework/pictures/Telegram_mF4OU8TK9I.png" />

---
## Интеграция с Allure TestOps
### Тест кейсы
<img align="center" src="https://github.com/Lexzender/luma_UI_test_framework/blob/main/luma_UI_test_framework/pictures/test%20cases.png" />

### Дашборд
<img align="center" src="https://github.com/Lexzender/luma_UI_test_framework/blob/main/luma_UI_test_framework/pictures/dashboards.png" />

### История запусков
<img align="center" src="https://github.com/Lexzender/luma_UI_test_framework/blob/main/luma_UI_test_framework/pictures/Launches.png" />

### Тестовые артефакты
<img align="center" src="https://github.com/Lexzender/luma_UI_test_framework/blob/main/luma_UI_test_framework/pictures/test_results.png" />

---
## Интеграция с Jira
<img align="center" src="https://github.com/Lexzender/luma_UI_test_framework/blob/main/luma_UI_test_framework/pictures/Jira.png" />
