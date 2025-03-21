# Создание [дашборда](https://public.tableau.com/views/Unicorns_16791633199530/Dashboard1?:language=en-US&:sid=FC34DAC2FE14440A8EBE6CBAC9602269-0:0&:redirect=auth&:display_count=n&:origin=viz_share_link) для анализа соновных показателей компаний-единорогов.
  
## Данные
Данные о компаниях-единорогах (https://disk.yandex.ru/i/Qdyir2rq2hydsg).  
Компании единороги - это частные компании, стоимость которых превышает 1 млрд. долларов по состоянию на 1 января 2023 г. Данные включают текущую оценку стоимости каждой компании, размер привлеченных инвестиций, страну, в которой зарегистрирована компания, отрасль, в которой работает компания-единорог, компании-инвесторы, годы, в которые компания привлекла инвестиции и когда стала единорогом, описание деятельности, ссылки на сайт, адреса, стадии инвестирования.  
Также будем использовать датасет с компаниями-инвесторами: https://disk.yandex.com/d/BeQ_h19NGir4oA  
Источники данных: https://www.cbinsights.com/research-unicorn-companies и https://news.crunchbase.com/unicorn-company-list/  

## Описание полей:

### Unicorns: 
'Company' - название компании  
Valuation (B) - оценка стоимости компании, млрд. долларов  
Date Joined - дата, когда компания стала единорогом  
Country - страна регистрации компании  
City - город регистрации компании  
Continent - континент регистрации компании  
Industry - отрасль, в которой работает компания  
Select Investors - инвесторы, которые проинвестировали команию, перечислены через запятую  
url - адрес веб-сайта компании  
founded_year - год основания компании  
stage - раунд инвестирования, на котором находится компания  
total_funded - размер инвестиций в компанию, млрд. долларов  
description - описание деятельности компании  
hq_address - адрес главного офиса 

### Investors: 
Company - название компании  
Select Investors - инвесторы, которые проинвестировали команию, каждый инвестор — в отдельной строке 

## Цель
Провести анализ показателей компаний-единорогов и ответить на следующие вопросы:

- У каких компаний наибольший ROI (return on investment)?
- Сколько обычно компании требуется времени, чтобы стать единорогом?
- В каких странах больше всего компаний-единорогов? Можно ли выделить города - отраслевые хабы?
- Какие компании-инвесторы проинвестировали больше всего компаний-единорогов?
