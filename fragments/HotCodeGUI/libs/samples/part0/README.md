Первое практическое задание акцентирует ваше внимание в основном на самом процессе форк -> решение -> пулл реквест.
Непосредственно в проекте есть всего одна Activity (MainActivity) и есть разметка для этой активности (res/layout/activity_main.xml), но не вызывается метод активности, который устанавливает эту разметку.
Метод Activity#setContentView() принимает в качестве аргумента числовой идентификатор разметки, который генерируется и хранится в классе R.
В нашем случае это R.layout.activity_main.
Установка разметки производится в методе жизненного цикла активности onCreate() после вызова super.onCreate().