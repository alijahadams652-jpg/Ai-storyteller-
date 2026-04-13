# Ai-storyteller-
Ai stories 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>AI Story Generator</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #0f0f0f;
      color: white;
      text-align: center;
      padding: 40px;
    }

    h1 {
      font-size: 40px;
      margin-bottom: 10px;
    }

    input {
      width: 80%;
      padding: 15px;
      margin-top: 20px;
      border-radius: 10px;
      border: none;
      font-size: 16px;
    }

    button {
      margin-top: 15px;
      padding: 15px 25px;
      border: none;
      border-radius: 10px;
      background: #ff2d55;
      color: white;
      font-size: 16px;
      cursor: pointer;
    }

    button:hover {
      background: #ff4d73;
    }

    .output {
      margin-top: 30px;
      background: #1c1c1c;
      padding: 20px;
      border-radius: 12px;
      width: 80%;
      margin-left: auto;
      margin-right: auto;
      min-height: 150px;
      text-align: left;
      white-space: pre-line;
    }
  </style>
</head>

<body>

  <h1>AI Story Generator</h1>
  <p>Type a topic (crime, horror, romance, motivation)</p>

  <input id="topic" placeholder="e.g. crime boss betrayal">

  <br>
  <button onclick="generateStory()">Generate Story</button>

  <div class="output" id="output">
    Your AI story will appear here...
  </div>

  <script>
    function generateStory() {
      let topic = document.getElementById("topic").value;

      if (!topic) {
        document.getElementById("output").innerText = "Please enter a topic.";
        return;
      }

      let story = `Hook: Nobody in the city ever talked about ${topic}... but everyone knew the truth.

It started late one night when everything went wrong.

A man stepped into the shadows tied to ${topic}, and nothing was ever the same again.

People said it was impossible, that no one survives that world.

But what happened next changed everything...

Final twist: The truth behind ${topic} was never what anyone expected.`;

      document.getElementById("output").innerText = story;
    }
  </script>

</body>
</html>
