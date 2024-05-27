# Гайд по формализации текста в текстовом редакторе Latex.
## Начнём с того, что разберем базовые варианты формализации информации, которые вы встретите:**

1. Идентификаторы ( := ) - используются для указания другого названия, рассматриваемого вами понятия или сущности, или для определения вашего понятия. Например: ":= [knowledge base]"

2. Отношения ( => ) - используются для разбиение понятия на его составляющие, указание различных аннотаций, пояснений, авторов, библиографически ссылок и так далле.

### К основным видам отношений, которые вы можете встретить относятся:

- **Разбиение** - используется в случае, когда элементы, на которые вы разделяете ваше понятие, не связаны между собой
  
**Пример:**
  
  SC-код

  => разбиение*:

  {
  - SCn-код
  - SCg-код
  - SCp-код
  - SCs-код

  }
  
Каждая из этих вариаций SC-кода не пересается ни с какой другой, так как каждая из них представляется по-разному.
   
- **Декомпозиция** - используется в случае, когда вы не уверены, что элементы, на которые вы разделяете ваше понятие, не связаны между собой, однако вы понимаете, что определённое отличие есть.

**Пример:**

База знаний Метасистемы OSTIS

=> декомпозиция*:

{
- Формальная теория ostis-систем
- Стандарт ostis-систем
- Стандарт методик и средств поддержки жизненного цикла ostis-систем

}

Как вы видите, здесь нельзя с точностью сказать, насколько тесно связаны понятия, на которые мы декомпозируем, поэтому использовали именно такой метод. Идём далее...

- **Включение** - используется в случае, когда элементы, на которые вы разделяете ваше понятие, связаны между собой.

**Пример:**

образованная кибернетическая система

=> включение*:

- кибернетическая система, основанная на знаниях
- кибернетическая система, управляемая знаниями
- целенаправленная кибернетическая система
- гибридная кибернетическая система
- потенциально универсальная кибернетическая система

Здесь заметно, что понятия, которые описывают *образованную кибернетическую систему* тесно связаны между собой. Могу сказать, что на начальномм этапе работы с формализацией текста, лучше всего использовать *декомпозицию*, так как шанс того, что вы ошибетесь будет меньше. Также важно заметить, что при *отношении включения* не используются фигурные скобки: {}

- **Обобщенная декомпозиция** - используется почти так же, как и *декомпозиция*, однако здесь уже используется меньшее количество понятий, на которые бы разбиваете.

**Пример:**

менеджер многократно используемых компонентов ostis-систем

=> обобщенная декомпозиция*:

{
- база знаний менеджера многократно используемых компонентов ostis-систем
- решатель задач менеджера многократно используемых компонентов ostis-систем
- интерфейс менеджера многократно используемых компонентов ostis-систем
  
}

Ёще при использовании различных видов отношений, вы можете использовать свои слова, однако они должны быть использованы в Именительном падеже:

**Пример:**

=> цель*:

=> характеристика*:

И так далее...

Также вы можете использовать какое-либо уточнение, по которому вы разбиваете понятие:

**Пример:**

интеллектуальная компьютерная система нового поколения

=> разбиение*:

Подсистемы

:= {
- предметная (основная) подсистема
- интеллектуальный пользовательский интерфейс
- интеллектуальная подсистема адаптивного управления диалогом с конечным пользователем
- интеллектуальная help-система для информационного обслуживания и обучения конечных пользователей предметной подсистемы, которые, начиная работать с системой, не обязаны иметь сразу высокую квалификацию
- интеллектуальная подсистема управления проектированием интеллектуальной системы, которая координирует деятельность разработчиков предметной подсистемы
- интеллектуальная подсистема управления информационной безопасностью предметной подсистемы
  
}

Если же вы хотите как-то *уточнить* или *пояснить* информацию об описываемом понятии, вы можете использовать соответствующее отношение:

=> уточнение*:


[текст]

=> пояснение*:

[текст]

Обратите внимание на то, что в данном случае используются квадратные скобки и внутри текст. Это объясняется тем, что, когда мы используем [], то используем занесенную информацию как комментарий, то есть отдельным понятием она не являтся.

На SCg-коде это бы выглядело так: 

![image](https://github.com/MikhailOstrov/1-st/assets/144333910/817d38b3-8693-440c-9a39-9283db2928dc)

## Теперь перейдем к самой статье. Для ее поиска рекомендуется использовать *google scholar*. Поиск можно проводить как и по предметным областям монографии, так и по отдельным понятиям. Вы должны понимать, что целью вашей работы является дополнение уже существующих понятий и добавление новых. 
### Начнем разбирать статью:

C полным текстом статьи, рассматриваемой мной можно ознакомиться здесь: 

[bolshie-dannye-i-glubokoe-mashinnoe-obuchenie-v-iskusstvennyh-neyronnyh-setyah.pdf](https://github.com/MikhailOstrov/1-st/files/15455613/bolshie-dannye-i-glubokoe-mashinnoe-obuchenie-v-iskusstvennyh-neyronnyh-setyah.pdf)

Рассмотрим первое, что попадается на глаза: 

![image](https://github.com/MikhailOstrov/1-st/assets/144333910/5445a771-c761-4165-af62-d47fcd2c2a8e)
 
Из данного на скриншоте можно выделить 3 отношения, которые будут в самом начале нашей формализации: автор, аннотация и ключевые слова. По желанию можно дополнительно указать информацию об авторе, указанную под названием статьи. Открываем **LATEX**:

### На данном этапе будем изменять section1 из вашего *скопированного* проекта. Так вот всё оно выглядит.  

![image](https://github.com/MikhailOstrov/1-st/assets/144333910/5ec04df4-6f40-4906-8bd5-cc7d29166519)

### Можем удалить всё не нужное, до этого момента:

![image](https://github.com/MikhailOstrov/1-st/assets/144333910/0c1dc90c-4a68-4ec1-af9e-20cf3b9998b4)

### Разберемся как же вообще заполнять формализованным текстом ваш проект:

\scnheader{} - название вашего понятие 

\scnidtf{} - определение или другое название ( := )

\begin{scnrelfromlist}{библиографическая ссылка} & end{scnrelfromlist}  - В основном используется для указания библиографических ссылок. Во вторых {} скобках вы можете использовать нужное вам отношение разбиения. 

\scnitem{} - для добавления точки

\scntext{}{} - можно использовать для добавления ссылки, а также аннотации, цитаты, пояснения и уточнения, так как, как вы заметили, текст расположен в [] скобках.

\begin{scnsubdividing} & \end{scnsubdividing}- для указания разбиения



### Начинаем заносить информацию: 













=> автор*:
- Тихонов А.А.
  
=> аннотация*:

  [в статье раскрываются понятия Больших данных и глубокого машинного обучения искусственных нейронных сетей, а также описание областей их применения. Затрагивается проблема необходимости эволюции нейронных сетей посредством изменения их архитектуры и принципа работы]

=> ключевые слова*:
- анализ
- Большие данные
- глубокое машинное обучение
- визуализация
- нейронная сеть

=> библиографический источник*:

- Денисова О.О. и Мухутдинов Э.А. «Большие данные – это не только размер данных» // Вестник 
технологического университета, т. 18, № 4, p. 5, 2015.

=> библиографическая ссылка*:

- Себрант А. «Что такое Big Data и почему это страшно интересно,» 06.03.2014. [Электронный 
ресурс]. Available: http://www.youtube.comm/watch?v=zsUKYfXjpvo&list=WL&index=6, дата 
обращения: 22.03.2018.
- Сербант А. «Data S ie e, черные ящики – и почему вам сильно повезло,» 15.09.2015. 
[Электронный ресурс]. Режим доступа: 
http ://www.y utube. m/wat h?v=zvGeLvWZ7yQ&li t=WL&i dex=8/ (дата обращения: 22.03.2018).
- «Большие данные (Big Data),» 24.10.2017. [Электронный ресурс]. Available: 
http://tadvi er.ru/a/125096, дата обращения: 22.03.2018.
- Хайкин С. Нейронные сети: Полный курс, 2-ое ред., Издательский дом Вильямс, 2006, p. 1104.
- «Шпаргалка по разновидностям нейронных сетей. Часть первая. Элементарные конфигурации,» 
03.10.2016. [Электронный ресурс]. Режим доступа: http ://tpr ger.ru/tra lati / eural-network-zoo1/ (дата обращения: 22.03.2018).
- «Искусственная нейронная сеть,» 11.02.2018. [Электронный ресурс]. Режим доступа: 
https://ru.wikipedia.org/wiki/%D0%98%D1%81%D0%BA%D1%83%D1%81%D1%81%D1%82%D0%
B2%D0%B5%D0%BD%D0%BD%D0%B0%D1%8F_%D0%BD%D0%B5%D0%B9%D1%80%D0%B
E%D0%BD%D0%BD%D0%B0%D1%8F_%D1%81%D0%B5%D1%82%D1%8C/ (дата обращения: 
22.03.2018).
- Редозубов А.Д. «Мозг - это не нейронные сети,» 07.10.2016. [Электронный ресурс]. Режим 
доступа: http ://www.y utube. m/wat h?v=7 6YUJ0JuqI&list=WL&t=1s&index=27/ (дата 
обращения: 22.03.2018).
- Редозубов А.Д. «Логика мышления. Часть 1,» 29.08.2012. [Электронный ресурс]. Режим доступа: 
https://www.youtube.com/watch?v=0v5OwZx x7M, (дата обращения: 22.03.2018).
- Редозубов А.Д. «Логика сознания. Вступление,» 22.08.2016. [Электронный ресурс]. Режим 
доступа: http ://habrahabr.ru/p t/308268/, (дата обращения: 22.03.2018).
- Редозубов А.Д. Логика эмоций, 2012, p. 317.
- Развина Э. «Вспомнить все… А если это нереально?,» 27.12.2014. [Электронный ресурс]. Режим 
доступа: http ://www.b17.ru/bl g/15224/, (дата обращения: 22.03.2018)


**Большие данные**

:= [Big Data]

:= [технология обработки 
структурированных и неструктурированных данных]

=> следует отличать*:

{
- Большие данные
- структурированные базы данных
  
}

=> определяющая характеристика*:

{
- объём
  
  => уточнение*:
  
  [Большой объём данных (от 100 Тбайт) позволяет более точно находить различные связи для дальнейшего представления аналитики в агрегированном, понятном для чтения виде]
- вариативность
  
  => уточнение*:
  
  [Вариативность данных позволяет выявить зависимости там, где на первый взгляд их не стоит 
искать. Например, зависимость активности покупателей от погоды или зависимость 
продолжительности сна от потребления лекарств]

- скорость
- ценность

}

**наука о данных**

:= [Data Sience]

:= [наука, изучающая вопросы получения, обработки, анализа информации и предоставления этих данных в понятной форме]

=> результат развития*:

- технология машинное обучение
  

 **глубокое машинное обучение**

⊂ машинное обучение

 := [глубинное машинное обучение]

 := [deep machine learning]

 := [набор алгоритмов машинного обучения, основанный на нейросетях, которые пытаются моделировать высокоуровневые абстракции в данных, используя архитектуры, состоящие из множества нелинейных преобразований]

=> применение*:

{ 
 - искусственная нейронная сеть

}

 => задача*:

 {
 - [Представление изображения в виде вектора интенсивности значений на пиксель]
 - [Представление изображения в виде множества примитивов, областей определенной формы]
 - [Автоматизация процесса выбора и настройки признаков]

   => уточнение*:
   
   [обучение признаков проводится без учителя или с частичным привлечением учителя, используя для этого эффективные алгоритмы и иерархическое извлечение признаков]
   
 }


 **искусственная нейронная сеть**
 
 := [ИНС]
 
 := [математическая модель, а также её программное или аппаратное воплощение, построенная по принципу организации и функционирования биологических нейронных сетей — сетей нервных клеток живого организма]

 => неабходимое условие*:

 - обучение на большом объеме данных

 => характеристика*: 

 {
  - [автоматическое отделение нужных данных от ненужных]
  - [определение правильных признаков]
  - [потребность в больших вычислительных мощностях]
  - [исключение массу человеческих ошибок]

 }

 => пояснение*: 

 [Текущий уровень развития не даёт возможности целиком и полностью автоматизировать управление многими процессами только искусственными нейронными сетями, тем более, когда речь идёт о нестандартных ситуациях, хотя, ситуация является нестандартной, пока человек или ИНС не научатся в ней действовать]

**биологическая нейронная сеть**

:= [мозг]

=> принцип работы*: 

[Предполагается, что мозг работает не с аналоговыми, а с дискретными сигналами, таким образом, мозг (кора мозга) работает с конечным числом дискретных понятий. Вводится понятие интерференции информационной волны, способствующей формированию ключа воспоминаний (время, пространство, обстоятельства и пр.) для работы памяти с информацией, которую необходимо запомнить]

**сравнение***

∋ { 

- принцип работы мозга
- принцип работы комьютера

}

=> аналогия*:

[Для хранения информации используются 
различные метки (путь к файлу, время создания, различные теги и т.п.), для того, чтобы потом можно 
было легко найти файл даже по части имеющейся в ключе информации]

=> отличие*:

[Сохранение информации происходит не в конкретном месте, а распределено по всему 
мозгу. Подразумевается распределение не частей информации по разным местам, а 
сохранение всего жизненного объёма информации во множестве мест в головном мозге в 
кортикальных столбах]
