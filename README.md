# «Базы данных, их типы» Акиньшин С.Г.

### Задание 1

1. Для задач бюджетирования проектов и финансового анализа отчетности с прогнозированием рисков рекомендуется использовать реляционные СУБД, такие как Oracle, Microsoft SQL Server или PostgreSQL. 

Эти СУБД обеспечивают целостность данных и четкую структуру благодаря возможности определения ограничений на уровне таблиц и связей между ними. Кроме того, они поддерживают мощные инструменты для запросов и агрегирования данных, что необходимо для проведения анализа данных и формирования отчетности.

Для прогнозирования рисков также могут использоваться специализированные инструменты, такие как статистические пакеты R и Python, которые могут быть интегрированы с реляционными СУБД.

2. Если хеширование начало занимать длительное время, то можно рассмотреть использование алгоритмов хеширования, которые быстрее, чем используемый в настоящее время. Например, можно использовать алгоритмы, которые были разработаны для работы на современных процессорах с поддержкой инструкций AES-NI, такие как SHA-256 или SHA-3.

Кроме того, можно использовать библиотеки для оптимизации хеширования, такие как Intel Performance Libraries или OpenSSL. Эти библиотеки предоставляют оптимизированные реализации алгоритмов хеширования, которые могут значительно ускорить процесс.

Наконец, можно использовать параллельное вычисление хешей на множестве ядер процессора или даже на графических процессорах (GPU). Для этого можно использовать библиотеки, такие как OpenCL или CUDA, которые позволяют написать параллельный код для выполнения вычислений на GPU.

В зависимости от конкретной задачи и используемых технологий, можно выбрать оптимальный подход для ускорения работы хеширования.

3. Для лендингов, которые обычно имеют небольшой объем данных и не требуют сложных запросов, подойдут легковесные СУБД, такие как SQLite или MySQL. Они могут быть использованы для хранения информации о посетителях лендингов, а также для быстрого доступа к этим данным.

Для CRM же необходимо использовать более мощные СУБД, которые могут обеспечить хранение больших объемов данных и быстрый доступ к ним. Рекомендуется использовать реляционные СУБД, такие как PostgreSQL или MySQL с движком InnoDB, которые поддерживают транзакционность и могут обеспечить высокую скорость работы.

Также можно рассмотреть NoSQL СУБД, такие как MongoDB или Cassandra, которые могут хранить большие объемы данных и обеспечивать быстрый доступ к ним. Однако, они требуют особого подхода к проектированию схемы данных, что может быть затруднительно для некоторых проектов.

В любом случае, для обоих типов СУБД важно выбрать гибкую архитектуру и оптимизировать запросы для быстрого доступа к данным. Также рекомендуется использовать кэширование данных для дополнительной оптимизации работы.

4. Возможно использовать одну СУБД для лендингов и CRM, если требования к ним не очень высокие и объем данных не слишком большой. В таком случае можно использовать реляционную СУБД, такую как MySQL или PostgreSQL, с гибкой структурой данных и оптимизированными запросами.

Для создания лендингов и хранения информации о посетителях лендингов можно использовать одну базу данных, а для хранения информации о лидах и клиентах CRM - другую таблицу в той же базе данных. При этом, для удобства работы, можно использовать разные схемы для лендингов и CRM.

Для оптимизации работы можно использовать кэширование данных и индексы в базе данных. Также можно использовать горизонтальное и вертикальное шардирование для распределения нагрузки на базу данных.

Для решения данной задачи можно использовать любую реляционную СУБД, в зависимости от предпочтений и требований к производительности и масштабируемости.

5. Для создания базы данных по корпоративным нормам и правилам, обучающему материалу и прочему, рекомендуется использовать реляционную СУБД с простой и понятной структурой данных. 

Одним из наиболее популярных и широко используемых реляционных СУБД является MySQL. Она имеет простую и интуитивно понятную структуру, хорошую производительность и отлично подходит для создания баз данных различного размера и сложности. 

Также можно рассмотреть использование PostgreSQL, которая также имеет простую структуру, но отличается более продвинутыми возможностями по расширению функциональности и обработке сложных запросов.

Выбор СУБД для данной задачи зависит от требований к производительности, масштабируемости и безопасности, а также от опыта и предпочтений команды разработчиков.

6. В теории, можно использовать уже существующую СУБД из предыдущих задач для решения этой задачи. Однако, необходимо убедиться, что структура и требования к данным для отдела контроля качества не противоречат уже используемой СУБД и не создадут конфликтов при работе с данными.

Если уже используемая СУБД подходит для этой задачи, то лучше всего использовать ее вместе с новой базой данных. В таком случае, необходимо определить структуру данных для базы, создать новые таблицы и связи, а затем интегрировать их в существующую СУБД.

Если структура и требования к данным для отдела контроля качества отличаются от уже используемой СУБД, то может быть лучше создать отдельную базу данных для этой задачи, чтобы избежать конфликтов в будущем.

7. Для решения данной задачи наиболее подходящим типом СУБД является графовая СУБД. Графовые СУБД основываются на модели графов и хранят данные в узлах и ребрах графа, что позволяет эффективно работать с большим количеством связей между данными.

8. Для формирования маршрутов доставки материалов по объектам и распределения курьеров по маршрутам с доставкой документов, необходимо учитывать множество факторов, таких как географические данные, условия дорожного движения, время доставки и т.д. Графовая СУБД может эффективно обрабатывать такие сложные связи между данными и быстро находить оптимальные маршруты доставки и распределения курьеров.
Возможно, имеет смысл объединить СУБД отдела логистики и СУБД отдела закупок для того, чтобы обеспечить более эффективную работу обоих отделов и улучшить взаимодействие между ними. Однако, это зависит от конкретных потребностей компании и сложности задач, которые необходимо решить каждому отделу.

Если задачи отделов логистики и закупок сильно отличаются друг от друга и не связаны между собой, то возможно имеет смысл оставить у каждого отдела свою собственную СУБД. Если же задачи отделов связаны и существует потребность в обмене данными, то имеет смысл рассмотреть возможность объединения в одну СУБД.

9. Думаю, что это возможно. Лучшим вариантом может стать реляционная СУБД, такая как PostgreSQL или MySQL. Они обладают хорошей поддержкой связей между таблицами, что необходимо для решения задач контроля качества и логистики. Они также позволяют быстро работать с данными, а также поддерживают гибкую структуру, необходимую для задач CRM и девелопмента. Также реляционная СУБД может быть настроена для работы с большим объемом данных, что необходимо для задач бюджетирования проектов и прогнозирования рисков. В целом, реляционная СУБД может стать универсальным решением для всех перечисленных задач, при условии грамотного проектирования базы данных и ее оптимизации.


### Задание 2

2.1 Для того, чтобы пользователь мог успешно пополнить баланс счета телефона, необходимо выполнить следующие шаги:

1. Пользователь должен выбрать способ пополнения и ввести сумму пополнения.
2. Система должна проверить доступность выбранного способа пополнения и наличие достаточного количества средств для пополнения.
3. Если все условия выполнены, система должна запросить подтверждение операции у пользователя.
4. Пользователь должен подтвердить операцию пополнения.
5. Система должна выполнить транзакцию пополнения баланса счета пользователя с учетом комиссии и зачислить средства на счет.
6. Система должна отправить уведомление о результате операции пользователю.

Если в процессе выполнения одного из шагов возникнут ошибки или проблемы, то транзакция может завершиться неуспешно, и пользователь должен быть проинформирован об этом.

2.2 Если пополнение счёта телефона происходит через автоплатёж, то действия для завершения транзакции будут следующими:

1. Система автоматически проверяет наличие достаточного количества средств на банковской карте, связанной с автоплатежом.

2. Если на карте достаточно средств, система формирует запрос на проведение транзакции пополнения счета телефона.

3. Запрос на проведение транзакции отправляется в систему банка.

4. Банк производит проверку карточной транзакции на наличие ошибок и подтверждает возможность проведения платежа.

5. Если транзакция проходит успешно, банк переводит средства на счет телефона.

6. Система телефонной компании, в свою очередь, обновляет информацию о балансе счета телефона. 

После этих шагов пополнение счёта телефона будет выполнено автоматически.


### Задание 3

3.1. Некоторые из преимуществ SQL-систем по отношению к NoSQL:

1. Структурированные данные: SQL-системы, как правило, хранят данные в табличной форме с жестко определенными типами данных и структурами. Это позволяет гарантировать целостность и согласованность данных.

2. ACID-транзакции: SQL-системы гарантируют ACID-свойства транзакций, что означает, что каждая транзакция либо полностью выполняется, либо полностью откатывается, что обеспечивает целостность данных.

3. Мощные возможности запросов: SQL-системы имеют мощные возможности запросов, позволяющие вытаскивать данные из базы в самых разнообразных форматах и с различными условиями.

4. Гибкость: SQL-системы могут быть использованы для решения различных задач и иметь широкий диапазон применения, от маленьких проектов до больших систем.

5. Широкое распространение: SQL-системы широко распространены, имеют большое сообщество пользователей и разработчиков, а также множество документации и инструментов для работы с ними.

3.2 NewSQL-системы являются относительно новым классом баз данных, которые объединяют преимущества традиционных SQL-систем и NoSQL-систем. Они были созданы для обеспечения лучшей масштабируемости, производительности и надежности при работе с большими объемами данных. Вот несколько преимуществ, которые NewSQL-системы предоставляют по сравнению с SQL и NoSQL:

1. Масштабируемость: NewSQL-системы позволяют горизонтальное масштабирование, которое позволяет добавлять новые узлы к кластеру, когда это необходимо, обеспечивая при этом высокую доступность и расширяемость.

2. Производительность: NewSQL-системы используют оптимизированные алгоритмы для быстрого выполнения запросов, обеспечивая высокую производительность даже при работе с большими объемами данных.

3. Надежность: NewSQL-системы обычно имеют встроенные механизмы обеспечения отказоустойчивости и резервного копирования данных, что обеспечивает высокую надежность и защиту данных.

4. Гибкость: NewSQL-системы обычно позволяют использовать различные модели данных, включая реляционную и NoSQL, что обеспечивает гибкость в работе с различными типами данных.

5. Совместимость с SQL: NewSQL-системы поддерживают SQL-запросы и обладают теми же преимуществами, что и традиционные SQL-системы, включая полную ACID-совместимость, что обеспечивает надежность и консистентность данных. 

В целом, NewSQL-системы предоставляют лучшие возможности для работы с большими объемами данных, обеспечивая при этом высокую производительность, масштабируемость и надежность.

### Задание 4

Думаю, что требуется СУБД, которая способна обрабатывать многопоточные запросы и поддерживает горизонтальное масштабирование.

Как следует из информационных источников, из популярных СУБД, которые могут подойти для этой задачи, можно отметить Apache Cassandra, Apache HBase, Apache Spark SQL, Google Bigtable, и Amazon DynamoDB. Все эти СУБД могут обрабатывать большие объемы данных, а также поддерживают горизонтальное масштабирование и многопоточную обработку запросов.

Что касается модели распределенных вычислений, то здесь могут быть полезны такие инструменты как Apache Hadoop, Apache Spark, Apache Flink и Apache Storm. Они предоставляют распределенные вычислительные ресурсы, могут обрабатывать большие объемы данных и обеспечивать многопоточную обработку запросов.



