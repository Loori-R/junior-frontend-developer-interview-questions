# Вопросы, которые были заданы на собесах

1. CORE JS
    - типы данных
    - Замыкание
    - var vs let/const
    - хоистинг
    - приведение типов
    - блочный скоуп
    - какими методами массива можно найти элемент
    - все перебирающие методы массива
    - наследование ес5/es6 (написать)
    - для чего нужен Object.create
    - Object.create полифилл
    - для чего нужен prototype у конструкторов
    - нарисовать схему цепочки prototype
    - proto vs prototype
    - методы Function.prototype
    - можно ли переопределить контекст после bind
    - отличия стрелочных функций от обычных
    - es6 структуры данных
    - es6 фичи
    - что такое Set/Map
    - реализовать кастомный Set/Map в es5/es6 стилях
    - promise
    - Promise.all
    - Promise.race
    - asinc await
    - для чего используют Promise.resolve
2. HTML, CSS, animations
    - как можно сделать анимацию из js
    - requestAnimationFrame
    - keyframes
    - mobile first
    - двухколоночный макет(3х колоночный)
    - accessibility
    - семантика
    - семантика в HTML 4
    - веса селекторов (специфичность)
    - БЭМ
    - поток
    - позиционирование
3. DOM
    - DOM эвенты + стадии(баблинг, кэпчуринг таргет .. )
    - все возможные способы повесить обработчик на элемент
    - если на событии весит 2 обработчика как сделать что бы отработал только - первый?
4. REACT/REDUX
    - что такое React
    - плюсы реакта
    - когда происходит ререндер(в какой момент, как его остановить)
    - с чем сравнивается виртуальный дом(с предыдущим состоянием виртуального дома)
    - smart vs dump components, для чего, какую проблему решают
    - pure..vs component
    - shouldComponentUpdate(), как реализован в pure components, как работает shallowCompare
    - stateless component vs stateful component
    - можно ли реализовать аналог shouldComponentUpdate у функциональных - компонент (спойлер: можно, это новая фича React 16)
    - можно ли вообще юзать лайфсайкл хуки у функциональных компонентов (мнение интерьвьюера - нет, спойлер - можно! см. react-pure-lifecycle)
    - в чем преимущество функциональных компонент (версия интервьюера - быстрее работают)
    - что такое Redux
    - когда вообще появляется потребность в стэйт манагере в реакт проекте
    - store в redux - синхронный или асинхронный
    - все вспомогательные части Redux(как он работает)
    - флоу данных в Redux
    - что такое High Order Component(компонент наивысшего порядка)
    - схема react/redux
5. OTHER
    - ООП
    - Big-O
    - Event loop
    - Event handling
    - какие стадии рендера есть в ивент луп
    - OSI
    - HTTP
    - как работает HTTP\HTTPS как сервер понимает
    - как связан HTTP и TCP
    - how browser works
    - что происходит после ввода урл в строку поиска с поиском по кэшу , днс и тд
    - render pipline
    - Mime types
    - Response/request
    - таски/микротаски
    - написать кастомный fetch
    - отличие fetch/xhr
    - Синглтон es6
    - Синглтон es5
    - Инкапсуляция, наследования в JS
    - Инкпуляциб в js 3 способа
    - Паттерны
    - Поведенческие паттерны
    - синглотон и eммитер
    - что работает на emmiter паттерне в Core JS
    - что происходит когда создаешь объект через new
    - блокирующий js/css (что будет если в хедере 2гб css или js)
6. TASKS:
    - сделать класс, который принимает селектор CSS и крутит найденный элемент
    - реализовать свой Set/Map
    - counter (при каждом вызове функций +1)
    - Задача на алгоритм: дано два массива любых по величине, найти элемент который есть у обоих массивов и вернуть массив этого числа, все рассказать способы, а потом чтобы удовлетворил условие O(n).... Типа [1, 2, 7] [3, 2, 10, 100] вернуть [2]
    - Задачи на hoisting
        vax = 2;
        function x(x) {
            console.log(x);
            var x = 3;
            console.log(x);
        }

        vax = 2;
        function x(x) {
            console.log(x);
            x = 3;
            console.log(x);
        }
    - Сверстать меню (адаптивный)
    - Как вывести несколько элементов в дом (список из 10-20)
    - задачи на замыкание:
        - реализовать ф-цию подобие калькулятора, которая работает так:
            sum(1)(2)(3) = 6;
        - реализовать ф-цию fn которая работает так:
            const smth = fn([1,3,5,7,9]); // минимум 2 элемента, по возрастающей или убывающей, с константной дельтой между элементами
            smth(); // return 11
            smth(); // return 13
    - Проверка является ли строка палиндромом(устное решение)
    - Почти классическая с таймаутом (что выводит как исправить, спойлер var на let не поможет):
        var i = 0;
        while (i++ < 4) {
            setTimeout(() => {console.log(i);}, i * 10000);
        }
    - дан массив объектов [{a: ..., b: ..., c: ...}, ...], постороить в DOMе таблицу с соответствующими полями - т.е. каждый объект строкой в таблице, каждый ключ ячейкой, в посл ячейку кнопку которая в перспективе что-то делает с данными;
    - объединить 2 массива аргументов в функции в ES6 стиле без использования Array.prototype.concat и переборов всяческих;
