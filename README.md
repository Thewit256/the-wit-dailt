<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>The outspoken wit_Daily</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f5f5f5;
      color: #333;
    }
    header {
      background-color: #222;
      color: #fff;
      padding: 20px;
      text-align: center;
    }
    header img {
      width: 100px;
      height: 100px;
      border-radius: 50%;
      object-fit: cover;
    }
    .container {
      max-width: 800px;
      margin: 20px auto;
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    .story {
      margin-bottom: 40px;
    }
    .story h2 {
      color: #444;
    }
    .comments {
      margin-top: 20px;
    }
    .comment-box textarea {
      width: 100%;
      height: 80px;
      padding: 10px;
      border-radius: 5px;
      border: 1px solid #ccc;
    }
    .comment-box button {
      margin-top: 10px;
      padding: 10px 20px;
      border: none;
      background: #333;
      color: #fff;
      border-radius: 5px;
      cursor: pointer;
    }
    .comment-list {
      margin-top: 20px;
    }
    .comment {
      background: #f0f0f0;
      padding: 10px;
      margin-bottom: 10px;
      border-radius: 5px;
    }
  </style>
</head>
<body>
  <header>
    <img src="profile.jpg" alt="Author Photo" />
    <h1>The outspoken wit_Daily</h1>
    <p>By Adroni Emma</p>
  </header>  <div class="container">
    <div class="story">
      <h2>Leaning on a Twig</h2>
      <p><em>Posted on August 3, 2025</em></p>
      <p>"What should I do?" I thought to myself, my heart thumping like a drum in a war zone... (shortened for preview)</p>
    </div><div class="comments">
  <h3>Leave a Comment</h3>
  <div class="comment-box">
    <textarea id="comment-input" placeholder="Write your comment here..."></textarea>
    <button onclick="addComment()">Post Comment</button>
  </div>
  <div class="comment-list" id="comment-list">
    <!-- Comments will appear here -->
  </div>
</div>

  </div>  <script>
    function addComment() {
      const commentInput = document.getElementById("comment-input");
      const commentText = commentInput.value.trim();
      if (commentText !== "") {
        const commentList = document.getElementById("comment-list");
        const comment = document.createElement("div");
        comment.className = "comment";
        comment.innerText = commentText;
        commentList.appendChild(comment);
        commentInput.value = "";
      }
    }
  </script></body>
</html>
