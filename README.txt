
        При использовании аннотации @Transactional Spring берет на себя ответственность за открытие и закрытие транзакции.

 Можно так       List<Employee> employeeList = session.createQuery("from Employee"
                     , Employee.class).getResultList();

 А можно так     Query<Employee> query = session.createQuery("from Employee", Employee.class);
                 List<Employee>employeeList = query.getResultList();

     @Controller - специализированный @Component;
     @Repository - специализированный @Component. Данная аннотация используется для DAO;
                   При поиске компонентов, Спринг также будет регистрировать все ДАО с
                   аннотацией @Repository в Спринг Контейнере.



 @Service - посредник между DAO and Controller. Отмечает класс содержащий бизнес логику.
 @Service - специализированный @Component; При поиске компонентов, Спринг так же будет
            регистрировать все классы с данной аннотацией в Спринг Контейнере










    Spring Security в дальнейшем (SS) предоставляет функицонал для обеспечения безопасности приложения.
    Аутентификация - процедура проверки подлинности путем сравнения введеных user name-a и password с user name-ом и password-ом
                    хранящимся в БД.
    Авторизация - процедура проверки разрешений на доступ к тому или иному ресурсу.

