<div>
    В данном примере используется библиотека 
    <a target="_blank" href="https://github.com/parallax/jsPDF"><b>jsPDF Ver.1.4.0</b></a>
</div>

<div style="margin-top: 5%;">
    Очень часто при работе мне необходимо было при помощи библиотеки 
    jsPDF работать с русскоязычными символами (кириллицей). 
    Были небольшие танцы с бубном, чтобы все это дело заработало. 
</div>

<div style="margin-top: 5%;">
    В их документации подробно расписаны этот и другие кейсы, но я решил
    выделить именно этот способ работы с ней, так как часто с ним сталкиваюсь.
</div>

<div style="margin-top: 5%;">
    Чтобы постоянно не обращаться к документации я решил создать простенький 
    пример для работы с использованием этой библиотеки и с ее помощью создавать PDF-файлы,
    содержащие русскоязычные символы.
</div>

<div style="margin-top: 5%;">
    <p>Без лишней воды - от слов к делу.</p> 
    <p>Принцип действия и порядок следующий:</p>
    <ul>
        <li>
            Во-первых, для корректного отображения русскоязычных символов 
            нам необходимо скачать шрифт <b>PT Sans</b>. 
            В нашем случае он уже присутствует в папке с примером.
            Если Вы посмотрите на содержимое этой папки, то там просто находятся .ttf
            файлы, содержащие шрифты PT Sans-Web с различным начертанием.
        </li>
        <li>
            Во-вторых, был создан простой файл <b>script.js</b>, в котором мы
            создаем экземпляр класса jsPDF. В переменную <b>PTSans</b> заносится
            значение шрифта, которое мы должны были откуда-то взять <i>(пишу так,
            потому что на момент написания этого файла это значение надо было еще поискать).</i>
            Затем, добавляем наш новый шрифт, устанавливаем его для экземпляра класса jsPDF,
            пишем что угодно, что хотели бы видеть в сгенерированном файле PDF и сохраняем.
        </li>
        <li>
            В третьих, для примера я создал самый простой файл <b>jsPDF.html</b>,
            где подключил библиотеку <b>jspdf</b> и <b>script.js</b>.
        </li>
    </ul>
</div>

<div style="margin-top: 5%;">
    Очень важным моментом, на который я бы хотел заострить внимание, так это 
    указание в HEADER тега META с некоторыми атрибутами: 
    <xmp><meta http-equiv="Content-Type" content="text/html; charset=UTF-8" /></xmp>
</div>

<div style="margin-top: 5%;">
    Без данной настройки Вы не увидите рускоязычных символов на сгенерированной 
    странице PDF-файла.
</div>

<div style="margin-top: 5%;">
    Я очень надеюсь, что данный пример кому-нибудь когда-нибудь окажется полезен. 
    <b>Всем спасибо!</b>
</div>
