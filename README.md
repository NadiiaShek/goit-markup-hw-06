# goit-markup-hw-06


«B3» Выполнена разметка формы подписки на рассылку и всех её элементов в футере.

«B4» Выполнена разметка формы заявки и всех её элементов в модальном окне.

«B5» У всех инпутов в формах задан атрибут name.

«B6» Значения атрибута name описательные, точно характеризующий для чего это поле формы.

«B7» У всех инпутов есть связанный элемент <label>.

«B8» Инпутам задан атрибут placeholder если для него в макете есть текст-подсказка.

«B9» Кнопкам «отправки» форм задан атрибут type="submit".

«B10» Все новые иконки из форм добавлены в SVG-спрайт icons.svg.

Оформление
«C1» Выполнено оформление элементов формы подписки на рассылку в футере.

«C2» Выполнено оформление элементов формы заявки в модальном окне.

«C3» При получении инпутом фокуса, его рамка и иконка меняют цвет (как показано на макете).

«C4» Оригинальный чекбокс о принятии лицензионного соглашения в форме заявки скрыт.

«C5» Оформление «чекбокса» о принятии лицензионного соглашения сделано вручную, при помощи векторного изображения галочки из SVG-спрайта.

«C6» Для всех эффектов ховера и фокуса (цвет, фон, тень) сделаны переходы. Время - 250ms, функция распределения времени - cubic-bezier(0.4, 0, 0.2, 1).

Основним джерелом необхідної інформації для виконання ДЗ – конспект, відеоуроки А. Репети та живі вебінари з викладачем.
Формам необхідно приділяти особливу увагу – це інструмент для взаємодії користувача із сайтом. Наприклад, написання коментаря, вибір товару та оплата його, пошук тощо.
За допомогою форм розробники одержують дані користувача, обробляють ці дані або пересилають далі на сервер. Вивчення обробки даних виходить за межі нашого курсу HTML/CSS, але далі по курсу ви з цим познайомитеся.
Основні моменти, на які варто звернути увагу під час виконання ДЗ: 
Для приховування елементів на сторінках використовуємо патерн - visually-hidden ·
Уважно ознайомиться з матеріалом, який є у записах та конспекті - там є всі відповіді на запитання

Додаткові матеріали:
Ваша перша HTML форма - Your first form - Learn web development | MDN
developer.mozilla.orgdeveloper.mozilla.org
Your first form - Learn web development | MDN
Congratulations, you've built your first web form. It looks like this live: (24 КБ)



 Наполегливо рекомендую пройтися по своїй роботі та поправити, якщо раптом ще не здали. Ну або перевірити ще раз.
 Форма у футері. Зверніть увагу на те, як вона там позиціонована - вона притиснута до правого краю контейнера.
Позиціонування іконок у input. В основному це така конструкція: загальний div, в якому лежить label, input та svg-іконка. Іконка позиціонується абсолютом, але щодо свого батька -- div. Input -- це сусідній елемент для іконки. Не вірно (непотрібно) буде також прописати для інпуту position: relative. Можна вгадувати позиціонування до подібної візуальної відповідності, але це теж не буде технічно правильно.
Щоб правильно спозиціонувати іконку, є кілька варіантів, але найпростіший і зрозуміліший для вас - input і svg-іконку покласти в div. Цьому контейнеру дати position:relative. svg-position:absolute. І тепер буде зрозуміле і грамотне позиціонування іконки - вона через absolute дісталася з потоку документа, а div прийняв розміри input
Коли абсолютно позиціонуєте, не забувайте, що, як правило, треба дві точки. Наприклад top та left. Навіть якщо візуально нічого не зміниться.
Не забувайте, коли ставите, наприклад top:50% - це не зовсім центр, який хочеться. Щоб він був дійсним, додавайте transform: translateY(-50%);
Не забуваймо робити фокус на кастомному чекбоксі.







