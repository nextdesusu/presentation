#00:05 - 00:27
Привет всем, cегодня мы будем говорить о Mobx и Redux это фреймворки
использумые для управления состоянием приложения, в основном они используются в 
связке с такими фреймворками как: React, Vue js и Angular js.
#00:28 - 00:58
Теперь давайте поговорим об особенностях Mobx. Mobx: "battle tested" (имеется ввиду 
что он уже применялся в реальных проектах) он использовался во многих приложениях,
на протяжении многих лет, он прост и очень легок в изучении, его легко добавить в 
приложение и в основном для функционирования не требует от вас написания большого 
количества кода. Он быстр и не нагружает приложение.
#00:59 - 01:43
Теперь давайте поговрим об основных принципах Mobx. Mobx может иметь несколько 
"stores" ("хранилищ"), чем отличается от Redux потому как Redux не позволяет 
использовать более одного "хранилища", он требует от вас создания одного большого. 
"actions" (действия) могут быть "derived" (получены) без дальнейшего взаимодействия.
"action" (действие) это любой кусок кода который изменяет "state" (состояние),
все наследования, могут быть получены автоматически когда состояние изменяется.
#01:44 - 02:56
Теперь давайте поговорим о Redux, он "предсказуем", он помогает вам писать приложение 
таким способом, что оно ведет себя последовательно, и может работать в различных 
"окружениях", таких как: браузер и клиент. Он централизован, "централизирование" 
вашего приложения, его логики и состояния предоставляет вам такие возможности
как: "undo/redo" (отменить выполнение/повторить выполнение) вашего состояния, 
сохранение состояния, и многое другое. "debugabillity" (способность к отладке)
Redux обеспечивает вас "dev-tools" (инструментами разработчика) которые делают
легким отслеживаниетого где, когда и как состояние приложения изменилось, 
архитектура Redux, позволяет логировать такие изменения, а также использовать
так называемый "time-travel debugging". (дебаггинг во времени)
#02:57 - 03:25
Теперь об основных принципах Redux, он обладает одним большим хранилищем
для хранения состояния вашего приложения, сосотяние в хранилище неизменяемо
чем Redux отличается от Mobx где состояние изменяемо. "actions" (действия)
"invoke" (вызывают) изменения в состоянии и редукторы обновляют состояния
#03:26 - 04:47
Теперь к сравнению Redux, он в оснвном написан на JS в ES6, А Mobx написан 
на JS и TS вместе гдето на 60% на JS и на 40% TS. Хранилище информации
У Redux оно одно, а Mobx позволяет вам иметь несколько. Приложение
Redux в основном используется в больших, сложных приложениях которые требуют
"scaleability" (способность к расширению). Mobx в основном используется 
в маленьких и простых приложениях не всегда но чаще всего. "Scaleability" 
(способность к расширению) Redux в основном используется в приложениях
где "scaleability" необходимо. Mobx тоже неплох в этом плане но всетаки
похуже чем Redux. Теперь о производительности, Redux не обеспечивает
вашему приложению хорошую производительность он приносит ее в жерту 
простоте и в основном следует парадигме, функционального программирования
когда Mobx скорее следует парадигме импереативного программирования
и обеспечивает ваше приложение неплохой производительностью.
#04:48 - 06:07
Теперь к пирмерам кода. "props injection" (добавление информации) вы 
просто пишете клас contact-form-page и используете декораторы такие как,
@inject и @observer. И псоле вы можете легко получить к ним доступ через
this.props. props injection в Redux вы просто пишите специальную функцию
mapStateToProps и используете функцию connect чтобы "присоеденить" вашу
функцию к вашему класу, давая ему доступ к пропсам в этой функции. 
Хранилища, дествия и редукторы в Redux "action" (действие) это специальная
функция которые имеют "type" (тип) и "payload" (нагрузка), потомы вы пишете
редуктор, он в основном пишется так, он принимает action.type в качестве
аргумента и затем определяет что делать в зависимости от него.
Mobx версия, вы снова используете декоратор @action чтобы обернуть вашу 
функцию и делаете что-то похожее на то что показано в Redux.
#06:08 - 08:02
Теперь к заключению Redux и Mobx библиотеки используемые для управления
состоянием приложения, они делают это разными способами Redux использует
функциональный, а Mobx импереативный. В основном они используются в 
комбинации с "frontend" фреймворками, такими как React, Angular. Они
нужны чтобы сделать интерфейс более интерактивным, и показать как 
информация изменяется со временем. Mobx в основном предпочитают начинающие
из за его простоты, а Redux в основном предпочитают проффессионалы которые,
точно знают что им нужно, в последнее время стало ясно что Redux очень 
хорошо показал себя и стал популярным среди разработчиков, а Mobx не так
популярен, это не делает его плохим, так как вы все еще можете его 
использовать, он просто не так популярен, и я не знаю примеров больших 
компаний использующих его. Mobx и Redux это библиотеки с которыми
приятно работать и выбирать из них следует в зависмости от того, что
вам нужно. Вам нужна тестируемость, или производительность? Если
нужна тестируемость и простота вам скорее следует предпочесть Redux
а если нужна производительность следует выбрать Mobx.
Приятного изучения.
