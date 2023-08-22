<script lang="ts">
  import {
    Link,
    UnorderedList,
    ListItem,
    Tag,
    Accordion,
    AccordionItem
  } from 'carbon-components-svelte';
  import LogoGithub from 'carbon-icons-svelte/lib/LogoGithub.svelte';
  import Email from 'carbon-icons-svelte/lib/Email.svelte';
  import Phone from 'carbon-icons-svelte/lib/Phone.svelte';
  import Project from '../lib/project.svelte';
</script>

<div class="grid justify-items-center gap-20">
  <!-- header -->
  <div class="mt-40 grid justify-items-center">
    <p class="my-5">Java backend developer</p>
    <h1 class="font-bold text-7xl">Шпак Всеволод</h1>
  </div>

  <!-- content -->
  <div>
    <Tag>Английский - B2</Tag>
    <Tag type="red">Java</Tag>
    <Tag type="green">Spring Boot</Tag>
    <Tag type="blue">PostgreSQL</Tag>
    <Tag type="blue">MySQL</Tag>
    <Tag type="high-contrast">Git</Tag>
    <Tag type="outline">Linux</Tag>
    <Tag type="cyan">Docker</Tag>
    <Tag type="cool-gray">Hibernate</Tag>
    <Tag type="red">Redis</Tag>
  </div>
  <div class="grid gap-10">
    <div class="grid gap-10px">
      <p class="">Уралтех, Екатеринбург Декабрь 2022 - Июль 2023</p>
      <p class="font-semibold text-5xl">Опыт работы</p>
    </div>
    В качестве Java-разработчика я был ответственен за разработку серверной части веб-сайта по продаже
    фар, включая следующие задачи:
    <Accordion>
      <AccordionItem open title="Создание RESTful API">
        <p>
          Разработка эндпоинтов для управления товарными позициями, обработки заказов и управления
          пользовательскими данными. – Интеграция API с клиентской частью сайта.
        </p>
      </AccordionItem>
      <AccordionItem open title="Работа с базой данных: ">
        <p>
          Использование Spring Data JPA для создания и управления схемой базы данных в PostgreSQL. –
          Разработка запросов для извлечения, добавления, обновления и удаления данных.
        </p>
      </AccordionItem>
      <AccordionItem open title="Кэширование с помощью Redis">
        <p>
          Имплементация кэширования наиболее часто запрашиваемых данных для оптимизации
          производительности.
        </p>
      </AccordionItem>
      <AccordionItem
        open
        title="Использование Docker для создания образов приложения и базы данных"
      >
        <p>
          Настройка и оптимизация контейнеров для гарантированной и надежной работы в различных
          средах.
        </p>
      </AccordionItem>
      <AccordionItem open title="Тестирование">
        <p>Разработка юнит и интеграционных тестов с использованием JUnit и Spring Boot Test.</p>
      </AccordionItem>
    </Accordion>
  </div>

  <div class="grid gap-10">
    <p class="font-semibold text-5xl">Проекты</p>

    <div class="grid gap-10 grid-cols-1 lg:grid-cols-2">
      <div class="lg:grid-col-span-2">
        <Project
          title="Консольные Шахматы на Java"
          gitlink="https://github.com/porunit/spring-studygroups-manager"
          gitname="ConsoleChess"
        >
          <p>
            Проект представляет себя реализацию классической игры в шахматы с консольным
            интерфейсом. Система базируется на клиент-серверной архитектуре, где сервер обеспечивает
            взаимодействие двух клиентов, участвующих в игре. Данные между клиентами и сервером
            передаются по протоколу TCP/IP.
          </p>
          <br />
          <p class="font-500 text-xl">Особенности:</p>
          <br />
          <UnorderedList class="ml-7">
            <ListItem>Консольный интерфейс</ListItem>
            <ListItem>Клиент-серверная архитектура</ListItem>
            <ListItem>Поддержка игры между двумя участниками</ListItem>
            <ListItem>Использование стандартных средств Java без сторонних библиотек</ListItem>
          </UnorderedList>
        </Project>
      </div>

      <Project
        title="Study groups manager"
        description="Данный проект - это сервис для управления группами учащихся который дает возможность
          видеть группы других пользователей, а так же добавлять, удалять и изменять свои группы
          а также искать наиболее популярные среди них. Кроме того, на сервисе можно смотреть на
          визуализацию групп на координатной оси, которые расположены там относительно указанных
          координат."
        gitlink="https://github.com/porunit/spring-studygroups-manager"
        gitname="spring-studygroups-manager"
      />

      <Project
        title="Headlights"
        gitlink="https://github.com/porunit/headlights"
        gitname="headlights"
      >
        <p class="font-500 text-xl">Основные технологии и инструменты:</p>
        <br />
        <UnorderedList class="ml-7">
          <ListItem>Spring Boot - основа приложения.</ListItem>
          <ListItem>Data JPA - для работы с базой данных.</ListItem>
          <ListItem>PostgreSQL - в качестве основной базы данных.</ListItem>
          <ListItem>Redis - для кеширования данных.</ListItem>
          <ListItem>Docker - для создания и управления контейнерами.</ListItem>
          <ListItem>JWT - для реализации системы авторизации.</ListItem>
        </UnorderedList>
      </Project>
    </div>
  </div>
  <div class="grid gap-10 w-full">
    <div class="grid gap-10px">
      <p class="">2022 - Данный момент</p>
      <p class="font-semibold text-5xl">Образование</p>
    </div>
    Университет ИТМО. Системное и прикладное программное обеспечение.
  </div>

  <!-- footer -->
  <div class="w-full dotted-spaced flex py-10 flex-col md:flex-row gap-5">
    <p class="font-semibold font-semibold">Шпак Всеволод</p>
    <div class="md:ml-auto flex gap-10px">
      <p class="font-semibold">Контакты:</p>
      <div class="flex items-center gap-10px">
        <LogoGithub />
        <Link target="_blank" href="https://github.com/porunit">GitHub</Link>
      </div>
      <div class="flex items-center gap-10px">
        <Phone />
        <Link target="_blank" href="tel: +7-(961)-401-11-04">+7-(961)-401-11-04</Link>
      </div>
      <div class="flex items-center gap-10px">
        <Email />
        <Link target="_blank" href="mailto: shpakyn.26@gmail.com">Email</Link>
      </div>
    </div>
  </div>
</div>

<style lang="scss">
  .dotted-spaced {
    background-image: linear-gradient(to right, #333 10%, rgba(255, 255, 255, 0) 0%);
    background-position: top;
    background-size: 10px 1px;
    background-repeat: repeat-x;
  }
</style>
