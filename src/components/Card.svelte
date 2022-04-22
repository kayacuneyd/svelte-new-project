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
      explanation: "Check me on UpWork Freelancer Platform.",
      platformLink: "http://www.upwork.com/",
    },
    {
      freelancePlatform: "Rimuut",
      platformImg: "static/images/rimuut.png",
      explanation: "Or hire me on Rimuut for your projects.",
      platformLink: "http://www.rimuut.com/",
    },
  ];

</script>

<div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
  {#each datas as data}
    <div class="col">
      <div class="card shadow-sm p-1">
        <div class="card-body text-center">
          <h3 class="card-title">{data.freelancePlatform}</h3>
          
          <a href={data.platformLink} target="_blank" class="btn platform-link"
            ><img
              src={data.platformImg}
              class="card-img-top card-image mx-auto"
              alt={data.freelancePlatform}
            /></a
          >
          <p class="card-text">
            {data.explanation}
          </p>
        </div>
      </div>
    </div>
  {/each}
</div>