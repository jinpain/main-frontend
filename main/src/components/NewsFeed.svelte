<script>
  import News from "./News.svelte";
  import NewsModal from "./modals/NewsModal.svelte";

  const newsList = [
    {
      title: "Первая новость",
      date: "30.05.2025",
      image: "/news.jpg",
    },
    {
      title: "Вторая новость, тоже очень интересная",
      date: "29.05.2025",
      image: "/news.jpg",
    },
    {
      title: "Еще одна важная новость",
      date: "28.05.2025",
      image: "/news.jpg",
    },
  ];
</script>

<div class="container pt-5">
  <h2 class="fw-bold">Главные новости <button class="btn btn-sm btn-success">Добавить новость</button></h2>
  <div class="row row-cols-3 pt-3">
    {#each newsList as news}
      <div class="col">
        <News {news} />
      </div>
    {/each}
  </div>
</div>

<NewsModal />
