# Дискуссии в процессе ревью

Иногда разработчики не будут принимать ваши замечания по ревью, просто не соглашаясь или жалуясь на вашу излишнюю строгость.


## Кто прав? {#who_is_right}

Когда разработчик не соглашается с вашим комментарием по его коду, для начала проверьте еще раз - возможно, он прав. Очень часто разработчик ближе к коду, чем вы и некоторые детали ему известны лучше. Насколько весомы его аргументы? Насколько они значимы с точки зрения развития кодовой базы в дальнейшем? Если разработчик прав, дайте ему об этом знать и закройте вопрос

Однако, автор кода не всегда бывает прав. В таком случае ревьюер должен пояснить подробнее, почему он считает свое замечание существенным. Хороший ответ демонстрирует понимание позиции разработчика и дополнительную информацию о том, почему этот комментарий все-таки имеет место.

В случае, когда ревьюер считает, что его предложение улучшит состояние кодовой базы и затрачиваемые усилия будут оправданы, он должен последовательно настаивать на изменениях. **Улучшение кодовой базы обычно происходит маленькими шагами**.

Иногда требуется несколько раундов переговоров, чтобы убедить разработчика. Всегда помните, что вы должны оставаться [вежливым](comments.md#courtesy). Дайте разработчику понять что *понимаете* его аргументы, но просто *не согласны* с ними.


## Расстраиваются ли разработчики {#upsetting_developers}

Иногда ревьюеры считают, что разработчик может расстроиться или обидиться, если продолжать настаивать на изменениях. Иногда это действительно случается, но, обычно это временно и в последствии, разработчик, как правило, благодарен что вы сумели улучшить предложенный им код. Обычно же, если вы [вежливы](comments.md#courtesy) в своих комментариях, то разработчики не расстраиваются вовсе, а все обиды надуманы ревьюером. Весь негатив обычно больше про то, [как](comments.md#courtesy) пишутся комментарии, а не про сам факт запроса изменений.


## "Сделаю позже" {#later}

Разработчики хотят чтобы дела были сделаны (что резонно) и, часто не хотят проходить еще один раунд ревью. Поэтому, типичные ответы на ваши комментарии будут связаны с обещаниями поправить что-то в следующем CL, и пожеланием к вам одобрить изменения сейчас. Некоторые разработчики добросовестно держат слово и оперативно делают новый CL со всеми исправлениями. Однако, как показывает практика, чем больше времени проходит с момента создания CL, тем меньше шансов что дополнительные фиксы когда-либо будут сделаны. И здесь дело не в лени или безответственности, просто у разработчиков очень много работы и они могли забыть о о своем обещании. Обычно, лучший способ добиться изменений - это сделать их сразу, перед тем, как код будет влит в общую кодовую базу, и задача перейдет в статус "сделано". Позволяя отложить исправления на позже вы серьезно ухудшаете состояние кодовой базы проекта.

Если CL привносит в код необязательную сложность, то CL должен быть исправлен, только если дело не касается [экстренных случаев](../emergencies.md). Если по ходу работы над CL были обнаружены дополнительные проблемы, которые не могут быть решены сейчас, то разработчик должен завести себе баг на исправление и, опционально, добавить TODO-комментарий в код со ссылкой на баг.


## Жалобы на строгость ревью {#strictness}

Если ранее ваши ревью были слабыми, а теперь вы стали более требовательны, некоторые разработчики будут сильно возмущены. Достаточная [скорость проведения ревью](speed.md) обычно сводит подобные жалобы на нет.

Иногда требуются месяцы чтобы все нелоразумения исчезли полностью, но в общем случае, разработчики начинают понимать значимость строгих ревью когда видят, как их код становится лучше.

Даже самые ярые противники строгих ревью могут стать вашими самыми большими союзниками, когда они на практике встретятся с ситуацией, доказывающей, что ваша жесткая позиция в ревью была правильной.


## Разрешение конфликтов {#conflicts}

Если вы следуете всем вышеуказанным правилам, но все равно случаются конфликты с разработчиками и вы не можете их решить, обратитесь к [Стандартам код-ревью](standard.md) для понимания практик и стандартов, которые могут помочь вам решить конфликт.
