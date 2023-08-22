<script>
  import {
    Header,
    SideNav,
    SideNavItems,
    SideNavMenu,
    SideNavMenuItem,
    SideNavLink,
    SideNavDivider,
    SkipToContent,
    Content,
    Grid,
    Row,
    Column,
    HeaderUtilities,
    HeaderGlobalAction,
    HeaderAction,
    HeaderPanelLinks,
    HeaderPanelLink,
    HeaderPanelDivider
  } from 'carbon-components-svelte';
  import Logout from 'carbon-icons-svelte/lib/Logout.svelte';
  import { SkeletonText } from 'carbon-components-svelte';
  import { goto } from '$app/navigation';

  import 'carbon-components-svelte/css/white.css';
  import './styles.css';
  import 'virtual:uno.css';
  import UserAvatarFilledAlt from 'carbon-icons-svelte/lib/UserAvatarFilledAlt.svelte';
  import { browser } from '$app/environment';

  let isSideNavOpen = false;
  let isOpen1 = false;
  /**
  
  Шпак Всеволод, Java backend developer
 +7-(961)-401-11-04
# shpakyn.26@gmail.com § GitHub Profile
Навыки
Английский - B2 Java
Spring Boot PostgreSQL, mySQL Git
Linux Docker Hibernate Redis
Опыт работы
Уралтех, Екатеринбург
Декабрь 2022 - Июль 2023
В качестве Java-разработчика я был ответственен за разработку серверной части веб-сайта по продаже фар, включая следующие задачи:
∙ Создание RESTful API:
– Разработка эндпоинтов для управления товарными позициями, обработки заказов и
управления пользовательскими данными.
– Интеграция API с клиентской частью сайта.
∙ Работа с базой данных:
– Использование Spring Data JPA для создания и управления схемой базы данных в
PostgreSQL.
– Разработка запросов для извлечения, добавления, обновления и удаления данных.
∙ Кэширование с помощью Redis:
– Имплементация кэширования наиболее часто запрашиваемых данных для оптимизации
производительности.
∙ Использование Docker для создания образов приложения и базы данных.
– Настройка и оптимизация контейнеров для гарантированной и надежной работы в различных средах.
∙ Тестирование:
– Разработка юнит и интеграционных тестов с использованием JUnit и Spring Boot Test.
Образование
2022 - Данный момент
Унивеситет ИТМО. Системное и прикладное программное обеспечение
  
  */
</script>

<Content>
  <Grid>
    <Row>
      <Column>
        <slot />
      </Column>
    </Row>
  </Grid>
</Content>
