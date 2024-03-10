### Описание XPath запросов на сайте http://online.sber.insure.  
  
#### XPath запросы на странице "Выбор полиса"  
  
| № | Кнопки | Поля ввода | Чекбоксы |Датапикеры| Остальное |  
| :-: | :-: | :-: | :-: | :-: | :-: |
1 | __"Квартира"__ -//h4[text()='Что будет застраховано?']/following::button[1] | __"Промокод"__ - //input[@formcontrolname='promoCode'] | __"Отчество отсутствует"__ //*[text()='Отчество']/following::mat-checkbox[1]| __"Дата начала"__ - //*[text()='Дата начала']/following::button[1] | __Логотип СБЕРСТРАХОВАНИЕ__ - //div[@class='sber-logo']   
2 | __"Дом"__ - //h4[text()='Что будет застраховано?']/following::button[2] | __"Фамилия"__ //input[@formcontrolname='lastName'] | __"Улица отсутствует"__ //*[text()='Улица']/following::mat-checkbox[1] | __"Дата выдачи"__ - //*[text()='Дата выдачи']/following::button[1]| __Хедер "Что будет застраховано?"__ - //h4[text()='Что будет застраховано?']  
3 | __"Сдается в аренду"(ДА)__ - //div[text()='Сдается в аренду']/following::button[1] | __"Имя"__ - //input[@formcontrolname='name'] | | __"Дата рожденья"__ - //*[text()='Дата рождения']/following::button[1] | __"Слайдер в блоке выбора суммы"__ - //div[@class='mat-slider-wrapper']  
4 | __"Сдается в аренду"(НЕТ)__ - //div[text()='Сдается в аренду']/following::button[2] | __"Отчество"__ - //input[@formcontrolname='middleName']| | | __Текстовый блок: "Мебель,техника и ваши вещи"__ //div[contains(text(),'Мебель')]  
5 | __"Расположена на первом или последнем этаже"(ДА)__ - //div[text()='Расположена на первом или последнем этаже']/following::button[1]| __"Дата рожденья"__ - //input[@formcontrolname='birthDate']| | | __Текстовый блок:"Падение летательных аппаратов и их частей"__ - //div[contains(text(),'Падение летательных')]  
6 | __"Расположена на первом или последнем этаже"(НЕТ)__ - //div[text()='Расположена на первом или последнем этаже']/following::button[2]| __"Серия"__ - //input[@formcontrolname='docSeries']| | | __1я колонка текстого блока:"Страховая защита включенная в программу"__ -  //h4[contains(text(),'Страховая защита')]/following::ul[1]  
7 | __"Установлена охранная сигнализация"(ДА)__ - //div[text()='Установлена охранная сигнализация']/following::button[1]| __"Номер"__ - //input[@formcontrolname='docNumber']| | | __2я колонка текстого блока:"Страховая защита включенная в программу"__ - //h4[contains(text(),'Страховая защита')]/following::ul[2]  
8 | __"Установлена охранная сигнализация"(НЕТ)__ - //div[text()='Установлена охранная сигнализация']/following::button[2]| __"Дата выдачи"__ - //input[@formcontrolname='docDate']  
9 | __"Применить"__ - //h4[text()='Промокод']/following::button | __"Кем выдан"__ - //textarea[@formcontrolname='docIssuer'] |  
10 | __"Оформить"__ - //h4[text()='Стоимость и срок действия']/following::button | __"Код подразделения"__ - //input[@formcontrolname='docDepartmentCode']| | | |  
11 | __"Заполнить по Сбер ID"__ - //h4[text()='Страхователь']/following::button| __"Город или населенный пункт"__ - //input[@formcontrolname='registrationCity']| | | |  
12 | __"Мужской"__ - //h4[text()='Страхователь']/following::button[3]| __"Улица"__ - //input[@formcontrolname='registrationStreet']| | |  
13 | __"Женский"__ - //h4[text()='Страхователь']/following::button[4]| __"Дом"__ - //input[@formcontrolname='registrationHouse'] | | |  
14 | __"Вернуться"__ - //div[@class='form-actions']/button[1]| __"Квартира"__ - //input[@formcontrolname='registrationFlat']| | |  
15 | __"Оформить"__ - //div[@class='form-actions']/button[2]| __"Телефон"__ - //input[@formcontrolname='contactPhone']| | |     