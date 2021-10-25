# firstSpringProject

* Проект создается Maven -> Create from archetype -> org.apache.maven.archetypes:maven-archetyoe-webapp.

* При создании папок важно папку resources, где будут лежать ресурсы, в том числе и applicationContext, пометить как Resources Root, а папку java с кодом проекта как Sorces Root (Правая клавиша мыши -> Mark Directory As).

* Bean - объект класса, создаваемый Spring'ом.

* В applicationContext.xml `<bean id="musicBean" class="ru.solomakhin.spring.RockMusic"> </bean> ` `musicBean` - уникальный id, который будем вводить при вызове спринга getBeans(), а `ru.solomakhin.spring.RockMusic` - путь к классу, объект (бин) которого будет создавать.

* `ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("applicationContext.xml");` - будет работать только если папка resources помечена как Resources Root.
