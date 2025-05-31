<script>
  let { news, eventCallback } = $props();
</script>

<button
onclick={() => eventCallback(news)}
  type="button"
  data-bs-toggle="modal"
  data-bs-target="#newsModal"
>
  <div class="news-text-block">
    <small class="text-muted">{news.date}</small>
    <h5 class="fw-bold">{news.title}</h5>
  </div>
  <img class="img-fluid rounded-3" src={news.image} alt="img not found" />
</button>

<style>
  .news-text-block {
    height: 100px;
    overflow: hidden;
  }

  button {
    all: unset;
  }
</style>
