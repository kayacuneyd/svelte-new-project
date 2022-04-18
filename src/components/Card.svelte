<script>
  export const datas = [
    {
      freelancePlatform: "Fiverr",
      platformImg: "static/images/fiverr.png",
      explanation: "See my gigs on Fiverr Freelancer Platform.",
      platformLink: "http://www.fiverr.com/",
    },
    {
      freelancePlatform: "UpWork",
      platformImg: "static/images/upwork.png",
      explanation: "You can check me on UpWork Freelancer Platform.",
      platformLink: "http://www.upwork.com/",
    },
    {
      freelancePlatform: "Rimuut",
      platformImg: "static/images/rimuut.png",
      explanation: "Or you can hire me on Rimuut for your projects.",
      platformLink: "http://www.rimuut.com/",
    },
  ];

  /* export let platformLink; */
</script>

<div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
  {#each datas as data}
    <div class="col">
      <div class="card shadow-sm p-1">
        <div class="card-body text-center">
          <h5 class="card-title">{data.freelancePlatform}</h5>
          <p class="card-text">
            {data.explanation}
          </p>
          <a href={data.platformLink} target="_blank" class="btn platform-link"
            ><img
              src={data.platformImg}
              class="card-img-top card-image mx-auto"
              alt={data.freelancePlatform}
            /></a
          >
        </div>
      </div>
    </div>
  {/each}
</div>

<!-- <style>
  .platform-link {
    text-decoration: none;
    background-color: grey;
  }
</style> -->
