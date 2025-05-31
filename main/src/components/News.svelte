<script>
  export let news
</script>

<div data-bs-toggle="modal" data-bs-target="#newsModal">
  <div class="news-text-block">
    <small class="text-muted">{news.date}</small>
    <h5 class="fw-bold">{news.title}</h5>
  </div>
  <img class="img-fluid rounded-3" src={news.image} alt="img not found" />
</div>

<style>
  .news-text-block {
    height: 100px;
    overflow: hidden;
  }
</style>
