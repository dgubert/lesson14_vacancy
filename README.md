
<h1 align="center">14 урок. Домашняя работа.<br>Тесты на страницу Вакансии компании <a href="https://ozerki.ru/vacancies/"> Озерки.</a></h1>


##  **Содержание:**

---

* [Технологии и инструменты](#технологии-и-инструменты)
* [Проверки](#проверки)
* [Запуск тестов в Jenkins](#-запуск-тестов-в-jenkins)
* [Allure Report](#--allure-report)
* [Уведомление в Telegram о результатах тестов](#-уведомление-в-telegram-о-результатах-тестов)

## Технологии и инструменты:

---


| Java                                                                                         | IntelliJ  <br>  Idea                                                                                                 | GitHub                                                                                                           | JUnit 5                                                                                                           | Gradle                                                                                                     | Selenide                                                                                                         | Selenoid                                                                                                                  | Allure <br> Report                                                                                                         | Jenkins                                                                                                          | Telegram                                                                                                            |
|:---------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| <a href="https://www.java.com/"> <img src="media/logo/Java.svg" height="50" width="50"/></a> | <a href="https://www.jetbrains.com/idea/"><img height="50" src="media/logo/Intelij_IDEA.svg" width="50"/></a> | <a href="https://github.com/"><img alt="Github" height="50" src="media/logo/GitHub.svg" width="50"/></a> | <a href="https://junit.org/junit5/"><img alt="JUnit 5" height="50" src="media/logo/JUnit5.svg" width="50"/></a> | <a href="https://gradle.org/"><img alt="Gradle" height="50" src="media/logo/Gradle.svg" width="50"/></a> | <a href="https://selenide.org/"><img alt="Selenide" height="50" src="media/logo/Selenide.svg" width="50"/></a> | <a href="https://aerokube.com/selenoid/"><img alt="Selenoid" height="50" src="media/logo/Selenoid.svg" width="50"/></a> | <a href="https://github.com/allure-framework"><img alt="Allure" height="50" src="media/logo/Allure_Report.svg" width="50"/></a> | <a href="https://www.jenkins.io/"><img alt="Jenkins" height="50" src="media/logo/Jenkins.svg" width="50"/></a> | <a href="https://web.telegram.org/"><img alt="Telegram" height="50" src="media/logo/Telegram.svg" width="50"/></a> |


Содержание [Allure-отчета](https://jenkins.autotests.cloud/job/dgubert_lesson14_vacancy/allure/#suites):
* Шаги теста
* Скриншот страницы на последнем шаге
* Page Source
* Логи браузерной консоли
* Видео выполнения автотеста


## <img height="25" src="media/pic/logo.png" width="25"/> Проверки:

---

- ✓ *[Проверка названия страницы](https://jenkins.autotests.cloud/job/dgubert_lesson14_vacancy/allure/#suites/0598bc41331f40ac0f38fe5d0c32bb00/1c28556ee444b478/)*
- ✓ *[Проверка наличия вакансий на странице](https://jenkins.autotests.cloud/job/dgubert_lesson14_vacancy/allure/#suites/0598bc41331f40ac0f38fe5d0c32bb00/14a613d3621c9b18/)*
- ✓ *[Проверка поиска вакансий](https://jenkins.autotests.cloud/job/dgubert_lesson14_vacancy/allure/#suites/0598bc41331f40ac0f38fe5d0c32bb00/1e4c6794abd12a0c/)*

## <img height="25" src="media/logo/Jenkins.svg" width="25"/> Запуск тестов в Jenkins:

---

**Сборка в [Jenkins](https://jenkins.autotests.cloud/job/dgubert_lesson14_vacancy/)**
- *browserName - браузер, по умолчанию chrome*
- *browserVersion - версия браузера, по умолчанию 126.0*
- *browserSize - размер окна браузера, по умолчанию 1920x1080*
- *remoteUrl - логин, пароль и адрес удаленного сервера Selenoid*

**Команда для запуска тестов**
```bash  
clean test --debug
-DbrowserName=${browserName}
-DbrowserVersion=${browserVersion}
-DbrowserSize=${browserSize}
-DselenoidUrl=${selenoidUrl}
```

## <img height="25" src="media/logo/Allure_Report.svg" width="25"/></a>  <a name="Allure"></a>Allure Report	</a>

---

## Основная страница отчёта

<p align="center">  
<img title="Allure Overview Dashboard" src="media/pic/allure_main.png" width="850">  
</p>  

## Тест-кейсы

<p align="center">  
<img title="Allure Tests" src="media/pic/allure_suites.png" width="850">
</p>



## <img alt="Allure" height="25" src="media/logo/Telegram.svg" width="25"/></a> Уведомление в Telegram о результатах тестов
____
<p align="center">  
<img title="Allure Overview Dashboard" src="media/pic/notification.png" width="550">  
</p>