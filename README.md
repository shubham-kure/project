<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AI Chat Assistant</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="container">
    <h1 class="title">AI Assistant</h1>
    <div class="chat-box">
      <div class="message user">Hello, who are you?</div>
      <div class="message bot typing">I'm your smart AI assistant.</div>
    </div>
    <div class="input-area">
      <input type="text" placeholder="Type your message..." />
      <button>Send</button>
    </div>
  </div>
  <style>
  {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  body {
    font-family: 'Segoe UI', sans-serif;
    background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #fff;
  }
  
  .container {
    background: rgba(255, 255, 255, 0.05);
    border-radius: 16px;
    backdrop-filter: blur(10px);
    box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
    width: 400px;
    max-width: 90%;
    padding: 20px;
  }
  
  .title {
    text-align: center;
    margin-bottom: 20px;
    font-size: 1.8rem;
    letter-spacing: 1px;
  }
  
  .chat-box {
    height: 300px;
    overflow-y: auto;
    padding: 10px;
    display: flex;
    flex-direction: column;
    gap: 12px;
    background-color: rgba(255, 255, 255, 0.05);
    border-radius: 10px;
    margin-bottom: 15px;
  }
  
  .message {
    padding: 10px 15px;
    border-radius: 15px;
    max-width: 80%;
    font-size: 0.95rem;
  }
  
  .user {
    align-self: flex-end;
    background: #6a82fb;
  }
  
  .bot {
    align-self: flex-start;
    background: #fc5c7d;
  }
  
  .typing::after {
    content: '|';
    animation: blink 1s infinite;
  }
  
  @keyframes blink {
    0%, 50%, 100% {
      opacity: 1;
    }
    25%, 75% {
      opacity: 0;
    }
  }
  
  .input-area {
    display: flex;
    gap: 10px;
  }
  
  input[type="text"] {
    flex: 1;
    padding: 10px;
    border-radius: 10px;
    border: none;
    outline: none;
  }
  
  button {
    background: #00c6ff;
    color: white;
    padding: 10px 15px;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    transition: background 0.3s ease;
  }
  
  button:hover {
    background: #0072ff;
  }
</body>
</html>
