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



 <p class="modal-title">Оставьте свои данные, мы вам перезвоним</p>
        <form>
            <lebel class="label-modale" for="user-name">Имя</lebel>
            <input 
            type="name" 
            class="model-input" 
            name="user-name" 
            placeholder="Введите имя"
            required
            minlength="2"
            id="user-name">
            
            <lebel class="label-modale" for="user-tel">Телефон</lebel>
            <input type="tel" class="model-input" name="user-tel" placeholder="+38 (067) 514-45-45" required
                pattern="[\+]\d{2}\s[\(]\d{3}[\)]\s\d{3}[\-]\d{2}[\-]\d{2}" title="+38 (067) 514-45-45" id="user-tel">
            
            <lebel class="label-modale" for="user-email">Почта</lebel>
                <input type="email" class="model-input" name="user-email" placeholder="Введите почту" required
                id="user-email">

            <lebel class="label-modale" for="text-comments">Комментарий</lebel>
            <textarea 
            type="text"
            class="modale-textarea" name="text-comments" 
            placeholder="Введите текст" id="text-comments">

            <input 
            type="checkbox" 
            class="checkbox-modale">
            <p class="text-chekbox-modale">Соглашаюсь с рассылкой и принимаю Условия договора</p>
                
            <button 
            type="submit" class="btn-send-modale">Отправить</button>
        </form>