---
layout: single
title: "Blog"
permalink: /blog/
---
> Latest from [@faizanansari541 on Medium](https://medium.com/@faizanansari541)

<style>
  .blog-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 20px;
    font-family: 'Segoe UI', sans-serif;
    margin-top: 20px;
  }

  .blog-card {
    border: 1px solid #ddd;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
    display: flex;
    flex-direction: column;
    background-color: #fff;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .blog-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
    cursor: pointer;
  }

  .blog-card img {
    width: 100%;
    height: 160px;
    object-fit: cover;
    border-bottom: 1px solid #eee;
  }

  .blog-card-content {
    padding: 12px;
    flex: 1;
  }

  .blog-card h3 {
    margin: 0 0 8px;
    font-size: 1.05em;
  }

  .blog-card p {
    margin: 0 0 8px;
    font-size: 0.9em;
    color: #555;
  }

  .blog-card small {
    color: #999;
    font-size: 0.8em;
  }

  .blog-card a {
    color: #2980b9;
    font-size: 0.85em;
    text-decoration: none;
  }
</style>

<div id="medium-blogs" class="blog-grid"></div>

<script>
  const mediumURL = "https://api.rss2json.com/v1/api.json?rss_url=https://medium.com/feed/@faizanansari541";

  fetch(mediumURL)
    .then(res => res.json())
    .then(data => {
      const container = document.getElementById("medium-blogs");

      data.items.slice(0, 7).forEach(item => {
        const title = item.title;
        const link = item.link;
        const pubDate = new Date(item.pubDate).toDateString();
        const snippet = item.description.replace(/<[^>]*>?/gm, "").slice(0, 160) + "...";
        const imgMatch = item.content.match(/<img[^>]+src="([^">]+)"/);
        const image = imgMatch ? imgMatch[1] : "https://cdn-icons-png.flaticon.com/512/5968/5968906.png";

        const card = `
          <div class="blog-card">
            <img src="${image}" alt="Blog Thumbnail">
            <div class="blog-card-content">
              <h3><a href="${link}" target="_blank">${title}</a></h3>
              <p>${snippet}</p>
              <small>📅 ${pubDate}</small><br>
              <a href="${link}" target="_blank">Read more →</a>
            </div>
          </div>
        `;
        container.innerHTML += card;
      });
    })
    .catch(err => {
      document.getElementById("medium-blogs").innerHTML =
        "<p style='color: red;'>⚠️ Unable to load Medium blog posts. Please try again later.</p>";
    });
</script>



