<script>
  import News from "./News.svelte";
  import NewsModal from "./modals/NewsModal.svelte";

  let selectedNews = $state({
    title: "",
    body: "",
    date: "",
    image: "",
  });

  const newsList = [
    {
      title: "Первая новость",
      body: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus minima eum quo saepe perspiciatis commodi id, harum sunt animi, molestiae similique nulla voluptate quisquam sed assumenda impedit natus? Ad, distinctio.",
      date: "30.05.2025",
      image: "/news.jpg",
    },
    {
      title: "Вторая новость, тоже очень интересная",
      body: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus minima eum quo saepe perspiciatis commodi id, harum sunt animi, molestiae similique nulla voluptate quisquam sed assumenda impedit natus? Ad, distinctio.",
      date: "29.05.2025",
      image: "/news.jpg",
    },
    {
      title: "Еще одна важная новость",
      body: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus minima eum quo saepe perspiciatis commodi id, harum sunt animi, molestiae similique nulla voluptate quisquam sed assumenda impedit natus? Ad, distinctio.",
      date: "28.05.2025",
      image: "/news.jpg",
    },
  ];

  function handle(value) {
    selectedNews = value;
  }

  function newNews() {
    (selectedNews.title = ""),
      (selectedNews.body = ""),
      (selectedNews.date = ""),
      (selectedNews.image = "");
  }
</script>

<div class="container pt-5">
  <h2 class="fw-bold">
    Главные новости <button
      onclick={newNews}
      class="btn btn-sm btn-success"
      data-bs-toggle="modal"
      data-bs-target="#newsModal">Добавить новость</button
    >
  </h2>
  <div class="row row-cols-3 pt-3">
    {#each newsList as news}
      <div class="col">
        <News {news} eventCallback={handle} />
      </div>
    {/each}
  </div>
</div>

<NewsModal {selectedNews} />
