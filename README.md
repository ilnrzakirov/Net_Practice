# Net_Practice
This project is a general practical exercise to let you discover networking.

For detailed information, refer to the **[subject of this project](https://github.com/ilnrzakirov/Net_Practice/blob/main/en.subject.pdf)**

<details>
<summary>Первый уровень, домашняя сеть</summary>
  <p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl1.png"></p>
  
  ### В изображении выше мы видим маску сети 255.255.255.0, что означает, адресс сети, в случаи A  и B =  104.95.23.0. Маска подссети подразумевает диапозон адресов  от 0 - 255 (2 зарезервированы), что ровняется 24 битам. 104.95.23.0/24. Что бы все заработала, надо адрес подсети сделать идентичным а имя хоста, последние 8 бит уникальными.
  
  <p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl1.11.png"></p>
  
 </details>
 
 <details>
<summary>Второй уровень, домашняя сеть</summary>
    <p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl2.png"></p>
  ### Все, как в предыдущем уровне. Адреса 127.0.0.0 - 127.255.255.255 нельзя использовать в локальных сетях (подробнее по ссылке https://ru.wikipedia.org/wiki/Localhost)
  
  <p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl2.1.png"></p>
 </details>

<details>
  <summary>Третий уровень, домашняя сеть</summary>
  
   <p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl3.png"></p>
  
  ### Подробнее о Switch можно прочитать [здесь](https://ru.wikipedia.org/wiki/%D0%A1%D0%B5%D1%82%D0%B5%D0%B2%D0%BE%D0%B9_%D0%BA%D0%BE%D0%BC%D0%BC%D1%83%D1%82%D0%B0%D1%82%D0%BE%D1%80)
  
  ### Важно что бы коммутатор работал в одной сети. Подбираем адреса с диапозона одной сети.
  
  <p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl3.1.png"></p>
  
</details>
      
<details>
<summary>Четвертый уровень, домашняя сеть и роутер</summary>
  
 <p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl4.png"></p>
 
  ### Подробнее о маршрутизаторе или роутер [здесь](https://ru.wikipedia.org/wiki/%D0%9C%D0%B0%D1%80%D1%88%D1%80%D1%83%D1%82%D0%B8%D0%B7%D0%B0%D1%82%D0%BE%D1%80)
  
  ### В этой задаче нам нужно подключить к сети роутер. Важно что бы интерфейс роутера и узлы находились в одной сети
  
 <p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl4.1.png"></p>
  
</details>

<details>
<summary>Пятый уровень, статические маршруты</summary>
 
 <p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl5.png"></p>
  
### Подробнее о статических маршрутах [здесь](https://ru.wikipedia.org/wiki/%D0%A1%D1%82%D0%B0%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B0%D1%8F_%D0%BC%D0%B0%D1%80%D1%88%D1%80%D1%83%D1%82%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F)
### Подробнее о сетевых шлюзах [здесь](https://ru.wikipedia.org/wiki/%D0%A1%D0%B5%D1%82%D0%B5%D0%B2%D0%BE%D0%B9_%D1%88%D0%BB%D1%8E%D0%B7)
  
### В данной задаче необходимо правильно прописать маршруты. Для узла А адрес интерфейса маршрутизатора узла Б и наоборот для узла Б. Остльаные изменение по предыдущим уровням.
  
 <p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl5.1.png"></p>
 </details>
 
 <details>
<summary>Шестой уровень, подключение к интернет</summary>

 <p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl6.png"></p>
  
 ### Для успешного подключения в адрес шлюза указываем адрес интерфейса маршрутизатора. А в маршрут интернета указываем адрес сети узла
  
 <p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl6.1.png"></p>
  
 </details>
<details>
<summary>Седьмой уровень, подключение узлов к друг другу через маршрутизаторы</summary>
  
 <p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl7.png"></p>
  
### Для успешного соединения узлов необходимо в шлюзе клиента С указать адрес интерфейса маршрутизатора R22. Аналогично для клиента А. Далее настроить маршруты между роутерами так что бы они перенаправляли к друг другу.
  
<p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl7.1.png"></p>
</details>
 
<details>
<summary>Восьмой уровень, подключение группы сетей к интернет</summary>
  
<p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl8.png"></p>
  
### Для успешного подключения офисные узлы надо разделить на подсети. Соответсвенно в маршрутах указать правильные адреса к интерфейсу роутера. Далее Роутеры соединяем в рамках одной сети. В маршрутах роутеров указываем перенаправление к друг другу. Адрес шлюза интернет указываем интерфейс роутера.
  
<p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl8.1.png"></p>
</details>

<details>
<summary>Девятый уровень, подключение группы сетей, которые подключены к друг другу маршрутизаторами, к интернет</summary>
  
<p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl9.png"></p>
  
### Для успешного соединения всех узлов друг другом, а так же, с интернет, нужно, для начала, настроить отдельные подсети. 
### Можно начать с соединение клиента А и Б через коммутатор далее соединить сеть с интерфейсом роутера. И прописать в маршрутах интернета адрес сети.
### Далее можно клиента С подключить к интернету. Для этого в маршрутах указываем адрес интерфейса роутера. Далее роутер подключаем к маршрутизатору которая имеет выход в интернет. Для этого в маршрутах указваем перенаправление к друг другу.
### Клиента Д аналогично клиенту С подключаем к сети!
 
<p><img src="https://github.com/ilnrzakirov/Net_Practice/blob/main/img/lvl9.1.png"></p>
  
 
