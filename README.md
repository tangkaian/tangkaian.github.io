<!DOCTYPE html>
<html>

<head>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      text-align: center;
      margin: 0;
      padding: 0;
    }

    h1 {
      color: #4CAF50;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
      font-size: 36px;
      margin-top: 50px;
    }

    h2 {
      color: #333;
      font-size: 24px;
      margin-top: 30px;
    }

    p {
      color: #666;
      font-size: 18px;
      line-height: 1.6;
      display: none;
      opacity: 0;
      transition: opacity 0.5s ease;
    }

    img {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      margin: 20px auto;
      display: block;
      object-fit: cover;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
    }

   .section {
      background-color: white;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      padding: 20px;
      margin: 20px;
      border-radius: 5px;
    }

   .highlight {
      color: #4CAF50;
      font-weight: bold;
    }

   .animated-border {
      border: 2px solid transparent;
      transition: border-color 0.5s ease;
    }
  </style>
</head>

<body>
  <video id="myVideo" controls>
  <source src="WeChat_20241011224552.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
<script>
  const video = document.getElementById('myVideo');
  video.play(); // 播放视频
  video.pause(); // 暂停视频
</script>
  <h1>这就是我，不一样的烟火</h1>
  <div class="section animated-border">
    <h2>个人简介</h2>
    <p id="introP">大家好！我叫汤凯安，是141的一员。我对心理有着浓厚的兴趣，并希望能了解相关知识。</p>
  </div>
  <div class="section animated-border">
    <h2>优势与热情</h2>
    <ul>
      <li><p id="commP">我具备良好的沟通能力。我善于倾听他人的心声，能够理解他人的感受，并且能够以平和、友善的态度与他人交流。我相信，只有通过良好的沟通，才能真正走进同学们的内心世界，了解他们的需求和困扰。我会成为同学们心灵沟通的<span class="highlight">桥梁</span>。</p></li>
      <li><p id="empP">我有较强的同理心。我能够设身处地地为他人着想，感受他人的痛苦和快乐。当同学们遇到困难和挫折时，我会给予他们充分的理解和支持，让他们感受到温暖和关怀。我希望能成为同学们心灵的<span class="highlight">守护者</span>。</p></li>
      <li><p id="knowP">我对心理学有着一定了解。我阅读过一些心理方面的文章，参加过一些心理学讲座，这些经历让我对心理有一定的掌握。我希望能够运用这些知识为同学们提供更专业的帮助。</p></li>
    </ul>
  </div>
  <div class="section animated-border">
    <h2>工作计划</h2>
    <ul>
      <li><p id="dailyP"><span class="highlight">我还没想好。</span></p></li>
         </ul>
  </div>
  <div class="section animated-border">
    <h2>结语</h2>
    <p id="concluP">我深知心理健康对于同学们的重要性，我愿意尽我所能，为同学们的心理健康保驾护航。我相信，通过我的努力和大家的支持，我们能够营造一个更加健康、和谐的班级心理环境，绝不辜负同学们的信任。希望大家能给我一个机会，请大家投我一票。谢谢大家！</p>
  </div>
  <script>
    // 获取所有要显示的段落
    const paragraphs = document.querySelectorAll('p');
    let currentParagraphIndex = 0;
    document.addEventListener('click', function () {
      if (currentParagraphIndex < paragraphs.length) {
        paragraphs[currentParagraphIndex].style.display = 'block';
        paragraphs[currentParagraphIndex].style.opacity = 1;
        currentParagraphIndex++;
      }
    });
  </script>
</body>

</html>
