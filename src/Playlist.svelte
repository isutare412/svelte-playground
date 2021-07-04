<script lang="ts">
  const playlist = [
    { title: "🐺🐶🐺", link: "https://youtu.be/OMtgcaAmCYQ" },
    { title: "Pomsky", link: "https://youtu.be/tCxXd4SnkIQ" },
    { title: "밀복탄", link: "https://youtu.be/w9pTeImPk-w" },
    { title: "Funny cats", link: "https://youtu.be/eX2qFMC8cFo" },
    { title: "Training cats", link: "https://youtu.be/5530I_pYjbo" },
  ];

  let currentPlayIndex = Math.floor(Math.random() * playlist.length);

  function onClickLink() {
    currentPlayIndex = Math.floor(Math.random() * playlist.length);
  }
</script>

<div>
  <p class="text-lg text-center my-3">
    <a
      class="hover:text-yellow-500"
      target="_blank"
      href={playlist[currentPlayIndex].link}
      on:click={onClickLink}>Show some cats and dogs</a
    >
  </p>
</div>
