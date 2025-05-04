<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Open Redirect Test</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            margin: 0;
            padding: 20px;
        }
        
        .marquee-container {
            width: 100%;
            overflow: hidden;
            white-space: nowrap;
            background: #333;
            color: white;
            padding: 10px 0;
            margin-bottom: 30px;
        }
        
        .marquee-text {
            display: inline-block;
            animation: marquee 11s linear infinite;
            font-size: 24px;
            padding-left: 100%;
        }
        
        @keyframes marquee {
            0% { transform: translateX(0); }
            100% { transform: translateX(-100%); }
        }
        
        .content {
            max-width: 800px;
            margin: 0 auto;
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 20px;
        }
        
        .boom-container {
            display: flex;
            align-items: center;
            gap: 20px;
        }
        
        .boom {
            font-size: 5rem;
            font-weight: bold;
            color: #ad1818;
            animation: blink 0.9s linear infinite;
        }
        
        .fire {
            font-size: 3rem;
            animation: fire-anim 0.8s linear infinite alternate;
        }
        
        @keyframes blink {
            0% { opacity: 0; }
            50% { opacity: 1; }
            100% { opacity: 0; }
        }
        
        @keyframes fire-anim {
            0% { transform: scale(1); opacity: 0.7; }
            100% { transform: scale(1.2); opacity: 1; }
        }
    </style>
</head>
<body>
    <div class="marquee-container">
        <div class="marquee-text">Open Redirect</div>
    </div>
    
    <div class="content">
        <div class="boom-container">
            <div class="boom">Boom</div>
            <div class="fire">🚀</div>
        </div>
    </div>
</body>
</html>
