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

### <code><img width="3%" title="Jenkins" src="https://github.com/Lexzender/Lexzender/blob/main/images/jenkins-original.svg"></code> Запуск проекта в Jenkins

1) Открыть [проект](https://jenkins.autotests.cloud/job/wiki_mobile_test_framework/)
2) Нажать "Build with Parameters"
3) Заполнить параметры 
4) Нажать "Build"
<img align="center" src="https://github.com/Lexzender/wiki_mobile_test_framework/blob/main/utils/pictures/jenkins_mob.png" />

---

## <code><img width="3%" title="Allure_Report" src="https://github.com/Lexzender/Lexzender/blob/main/images/Allure_Report.png"></code> Allure report
### После прохождения тестов результаты можно посмотреть в Allure отчете
<img align="center" src="https://github.com/Lexzender/wiki_mobile_test_framework/blob/main/utils/pictures/allure_mob.png" />

### В отчете для каждого теста указана мета информация, а также приложены результаты прохождения: видео, html страницы, скриншот после прохождения.
<img align="center" src="https://github.com/Lexzender/wiki_mobile_test_framework/blob/main/utils/pictures/allure_video_mob.png" />

### Пример прохождения mobile-теста
<img align="center" src="https://github.com/Lexzender/wiki_mobile_test_framework/blob/main/utils/pictures/test_dave_article.gif" />


---
## <code><img width="3%" title="Telegram" src="https://github.com/Lexzender/Lexzender/blob/main/images/tg.png"></code> Нотификация в Telegram
После прохождения тестов результаты будут отправлены в Telegram
<img align="center" src="https://github.com/Lexzender/wiki_mobile_test_framework/blob/main/utils/pictures/Telegram_HlyAwmC8KZ.png" />

---
## <code><img width="3%" title="AllureTestOps.png" src="https://github.com/Lexzender/Lexzender/blob/main/images/AllureTestOps.png"></code> Интеграция с Allure TestOps
### Тест кейсы
<img align="center" src="https://github.com/Lexzender/wiki_mobile_test_framework/blob/main/utils/pictures/testops_tk.png" />

### История запусков
<img align="center" src="https://github.com/Lexzender/wiki_mobile_test_framework/blob/main/utils/pictures/testops_mob_launches.png" />

### Тестовые артефакты
<img align="center" src="https://github.com/Lexzender/wiki_mobile_test_framework/blob/main/utils/pictures/testops_mob.png" />

---
## <code><img width="3%" title="Jira.png" src="https://github.com/Lexzender/Lexzender/blob/main/images/jira-original.svg"></code> Интеграция с Jira
<img align="center" src="https://github.com/Lexzender/wiki_mobile_test_framework/blob/main/utils/pictures/jira_mob.png" />
