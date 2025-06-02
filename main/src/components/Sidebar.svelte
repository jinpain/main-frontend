<div class="d-flex">
  <!-- Sidebar -->
  <div class="sidebar border-end">
    <ul class="nav flex-column">
      <li class="nav-item">
        <a class="nav-link" href="#">🏠 Рабочий стол</a>
      </li>

      <li class="nav-item">
        <a
          class="nav-link"
          data-bs-toggle="collapse"
          href="#patientsMenu"
          role="button"
          aria-expanded="false"
          aria-controls="patientsMenu"
        >
          👥 Пациенты
        </a>
        <div class="collapse" id="patientsMenu">
          <ul class="nav flex-column ms-3">
            <li class="nav-item"><a class="nav-link" href="#">🔍 Поиск</a></li>
            <li class="nav-item">
              <a class="nav-link" href="#">🆕 Новый пациент</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">📋 История</a>
            </li>
          </ul>
        </div>
      </li>

      <li class="nav-item">
        <a
          class="nav-link"
          data-bs-toggle="collapse"
          href="#scheduleMenu"
          role="button"
          aria-expanded="false"
          aria-controls="scheduleMenu"
        >
          🗓️ Расписание
        </a>
        <div class="collapse" id="scheduleMenu">
          <ul class="nav flex-column ms-3">
            <li class="nav-item"><a class="nav-link" href="#">Сегодня</a></li>
            <li class="nav-item"><a class="nav-link" href="#">Неделя</a></li>
          </ul>
        </div>
      </li>

      <li class="nav-item">
        <a
          class="nav-link"
          data-bs-toggle="collapse"
          href="#docsMenu"
          role="button"
          aria-expanded="false"
          aria-controls="docsMenu"
        >
          📄 Документы
        </a>
        <div class="collapse" id="docsMenu">
          <ul class="nav flex-column ms-3">
            <li class="nav-item">
              <a class="nav-link" href="#">Назначения</a>
            </li>
            <li class="nav-item"><a class="nav-link" href="#">Анализы</a></li>
            <li class="nav-item">
              <a class="nav-link" href="#">Направления</a>
            </li>
          </ul>
        </div>
      </li>

      <li class="nav-item">
        <a class="nav-link" href="#">📊 Статистика</a>
      </li>

      <li class="nav-item">
        <a class="nav-link" href="#">⚙️ Настройки</a>
      </li>

      <li class="nav-item">
        <a class="nav-link text-danger" href="#">🚪 Выход</a>
      </li>
    </ul>
  </div>
</div>

<style>
  .sidebar {
    min-height: 100vh;
    width: 300px;
    background-color: #f8f9fa;
    padding-top: 1rem;
  }
  .sidebar .nav-link {
    color: #333;
  }
  .sidebar .nav-link:hover {
    background-color: #e9ecef;
  }
</style>
