# Паттерны поведения
Pассматривают вопросы о связях между объектами и 
распределением обязанностей между ними. Для этого могут использоваться 
механизмы, основанные как на наследовании, так и на композиции.
## Interpreter (Интерпретатор)
Паттерн Interpreter определяет грамматику простого языка для проблемной области, 
представляет грамматические правила в виде языковых предложений и интерпретирует их 
для решения задачи. Для представления каждого грамматического правила паттерн 
Interpreter использует отдельный класс. А так как грамматика, как правило, имеет 
иерархическую структуру, то иерархия наследования классов хорошо подходит для ее 
описания.  

Структура:  
<img src="https://user-images.githubusercontent.com/107203406/235526310-ac7591a5-95fe-40d1-9e7f-5f389178c24c.png" width="40%" alt="image">  

### Задание
Cоздать простейший интерпретатор текстового редактора, позволяющий исправлять 
стандартные ошибки, допускаемые при подготовке обычных текстов.  
Как правило, человек при наборе текста в программе WORD не обращает внимания на 
соблюдение правил структурного оформления текстов, что вызывает некоторые 
трудности при чистовой верстке.  
Типичные структурные ошибки:
1. Множественные пробелы;
2. Использование дефиса вместо тире;
3. Использование в качестве кавычек символов “”, тогда как стандартом является 
использование «»;
4. Неправильное использование табуляторов
5. Наличие «лишнего» пробела после открывающей скобки, перед закрывающей 
скобкой, перед запятой, перед точкой;
6. Наличие множественных символов перевода строки  
Разработать грамматику и иерархию классов. Используя паттерн « Interpreter » 
провести синтаксический анализ текста и устранить перечисленные ошибки. 

### Решение

Диаграмма классов:
![diagram_classes](https://user-images.githubusercontent.com/107203406/235630323-3941c8d4-56b5-4680-a221-a6c0dfe4b7a0.png)


