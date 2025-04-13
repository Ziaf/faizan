---
layout: single
title: "📝 Blog"
permalink: /blog/
---

> Latest from [@faizanansari541 on Medium](https://medium.com/@faizanansari541)

<div id="medium-blogs" style="display: flex; flex-direction: column; gap: 20px; font-family: 'Segoe UI', sans-serif; margin-top: 20px;"></div>

<script>
  const mediumURL = "https://api.rss2json.com/v1/api.json?rss_url=https://medium.com/feed/@faizanansari541";

  fetch(mediumURL)
    .then(res => res.json())
    .then(data => {
      const container = document.getElementById("medium-blogs");
      data.items.slice(0, 6).forEach(item => {
        const title = item.title;
        const link = item.link;
        const pubDate = new Date(item.pubDate).toDateString();
        const snippet = item.description.replace(/<[^>]*>?/gm, "").slice(0, 180) + "...";
        const image = item.thumbnail || "https://cdn-icons-png.flaticon.com/512/5968/5968906.png";

        const card = `
          <div style="display: flex; flex-direction: row; border: 1px solid #ddd; border-radius: 8px; overflow: hidden; box-shadow: 0 1px 4px rgba(0,0,0,0.05);">
            <div style="flex: 0 0 160px;">
              <img src="${image}" alt="Blog Thumbnail" style="width: 100%; height: 100%; object-fit: cover;">
            </div>
            <div style="padding: 12px; flex: 1;">
              <h3 style="margin: 0 0 6px;">
                <a href="${link}" target="_blank" style="color: #2e86c1; text-decoration: none;">${title}</a>
              </h3>
              <p style="font-size: 0.9em; color: #555; margin: 0 0 8px;">${snippet}</p>
              <p style="font-size: 0.8em; color: #999;">📅 ${pubDate}</p>
              <a href="${link}" target="_blank" style="font-size: 0.85em; color: #2980b9;">Read more →</a>
            </div>
          </div>
        `;
        container.innerHTML += card;
      });
    })
    .catch(err => {
      document.getElementById("medium-blogs").innerHTML =
        "<p style='color: red;'>⚠️ Failed to load Medium blog posts. Please try again later.</p>";
    });
</script>
