# Материалы менторинга


#### 1. Знакомство, Установка ПО, Запуск проекта, Создание GitHub репозитория
- про курс и подход к изучению  
- установка java и как задать JAVA_HOME  
- понятия JVM, JRE, JDK, JIT и нужно ли их знать на собеседовании  
- как происходит запуск Java кода  
- создание первого проекта на Spring Boot  
- загрузка проекта на GitHub  
- примитивные типы в Java и сколько памяти они занимают  
- методы класса Object

#### 2. Основы Java ч.1
- сколько весят объекты  
- методы wait и notify  
- массивы  
- условные операторы if - else, switch  
- циклы for, while, foreach
- конвенция наименований в Java  
- сигнатура функций  
- модификаторы доступа  
- классы
- dto, анемичная модель  
- ключевое слово final  
- ключевое слово static  
- константы и enum’ы  
- принципы ООП  
- интерфейсы, абстрактные классы, чем отличаются и что стоит использовать
- для чего нужны default методы в интерфейсах  
- дженерики  
- иерархия исключений, какие исключения стоит использовать в проекте  
- иерархия коллекций
- сравнение ArrayList и LinkedList, сложность операций 

#### 3. Основы Java ч.2
- принцип работы HashMap и что спрашивают на собеседованиях  
- функциональные интерфейсы  
- встроенные фукнциональные интерфейсы в Java: predicate, consumer, supplier, function, bifunction  
- Stream API: промежуточные и терминальные методы, принцип работы, особенности  
- Optional: методы, правила работы с optional и best practices  
- сравнение объектов с помощью Compareable и Comparator
- сериализация, десериализация, интерфейс Serializable, глубокое клонирование  
- аннотации в Java, для чего нужны и как создать собственную аннотацию

#### 4. Системы сборки: Gradle, Maven
- обзор систем сборки проектов
- maven, основные понятия  
- состав pom.xml  
- super pom  
- репозитории  
- скоупы зависимостей  
- жизненные циклы maven  
- фазы, плагины  
- профили  
- создание проекта на maven и его публикация в локальный репозиторий
- gradle, основные понятия  
- преимущества gradle 
- скоупы зависимостей и их отличия от maven  
- gradle wrapper 
- создание проекта на gradle и его публикация в локальный репозиторий  
- загрузка проекта в публичный github репозиторий, для всеобщего доступа

#### 5. Spring Boot основы
- причины популярности Spring  
- что из себя представляет Spring Boot и для чего нужен  
- отличие Spring Framework от Spring Boot  
- что такое starter'ы и автоконфигурации  
- где хранится код starter'ов  
- аннотации @ConditionalOn***  
- аннотация @SpringBootApplication  
- технология Inversion of Control  
- способы создания Bean'ов, BeanDefinitionReader'ы  
- что из себя представляет Bean  
- паттерн Proxy 
- ApplicationContext  
- аннотации для инъекции bean'ов: @Autowired, @Qualifier, @Primary

#### 6. Жизненный цикл bean'ов в Spring
- скоупы
- bean lifecycle (жизненный цикл) 
- что происходит с момента запуска Spring приложения и до момента старта  
- создание собственного BeanPostProcessor'а для логирования времени выполнения запросов при указании специальной аннотации  
- отличие механизмов DynamicProxy и CGLib

#### 7. Spring WebMVC ч.1
- способы указания настроек в Spring  
- плейсхолдеры в файлах настроек (SpEL)   
- @Profile и @ConditionalOnProperty для управления созданием бинов  
- профили для применения настроек  
- аннотации @Value и @ConfigurationProperties  
- HTTP протокол, его поколения  
- структура HTTP, методы, статусы ответов  
- JSON формат  
- структура url
- REST и RESTful

#### 8. Spring WebMVC ч.2
- использование mapstruct  
- Jar, War, Fat-Jar
- паттерн FrontController и его реализация DispatcherServlet  
- WebFilter’ы и Spring Interceptor’ы  
- HttpServletRequest, HttpServletResponse  
- реализация собственных Spring Interceptor и @ControllerAdvice для логгирования входящего запроса и ответа  
- валидация в Spring, использование аннотаций для валидации запросов в контроллерах 
- BindingResult, ручная валидация с помощью сервиса Validator  
- валидация property
- создание собственного валидатора
- @ExceptionHandler'ы

#### 9. Spring Data JPA, liquibase
- запуск postgres с помощью docker-compose  
- подключение базы данных с помощью Spring Data JPA  
- liquibase, структура скриптов, служебные таблицы  
- поля для аудита записей в бд  
- добавление запросов через аннотацию @Query, применение JPQL, выполнение native SQL запросов  
- аннотации: @MappedSuperclass, @PrePersist и @PreUpdate  

#### 10. Spring Boot starter. AOP
- пагинация и сортировка при поиске по фильтру  
- аспектно-ориентированное программирование (AOP)
- библиотеки AOP, принцип работы, основные понятия
- виды аспектов: before, around, after
- ключевые слова pointcut'ов  
- влияние на производительности  
- best practices AOP  
- создание стартеров в Spring Boot 3  
- как заменить BeanPostProcessor на аспект для логгирования времени выполнения методов  
- создание собственного стартера логгирования входящих и исходящих web запросов
- best practices создания стартеров

#### 11. Docker, Kubernetes, Openshift
- технологии виртуализации  
- виртуальные машины vs docker контейнеры  
- dockerfile, docker image, docker container, dockerhub, volume  
- создание собственного docker образа и контейнера
- команды Dockerfile  
- docker-compose  
- сборка и запуск приложения в docker контейнере с помощью docker-compose
- публикация образа приложения на dockerhub  
- kubernetes, основные понятия, что нужно знать  
- запуск приложения в kubernetes на нескольких pod'ах с балансировкой нагрузки
- OpenLens IDE для kubernetes, просмотр логов
- OpenShift, что из себя представляет, что нужно знать

#### 12. Git, Gitflow
- системы контроля версий
- git, основные команды 
- практические сценарии работы с git  
- gtiflow  
- семаническое версионирование (semver)  
- git платформы: Github, Gitlab, Bitbucket

#### 13. CI/CD, Jenkins, ssh
- CI/CD  
- аренда собственного VPS сервера
- подключение к серверу по ssh  
- создание пользователя на удаленном сервере
- установка приложения на удаленный сервер  
- Jenkins  
- создание pipeline в Jenkins для сборки приложения по tag'у
- создание pipeline для разворачивания приложения на сервере с подстановкой настроек из внешнего репозитория

#### 14. Основы многопоточности
- системные потоки и потоки в Java  
- способы создания потока
- разница между процессом и потоком  
- до каких пор приложение остается запущенным  
- почему все Java приложения являются многопоточными  
- Stack и Heap память 
- Garbage Collection
- Java Memory Model (JMM)  
- реордеринг
- правила Happens Before
- когда нужно думать о потокобезопасности  
- создание immutable объектов