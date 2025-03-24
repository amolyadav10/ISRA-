<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ISRA vs. Chapter 25 Bar - Case Analysis</title>
    <link rel="stylesheet" href="styles.css">
    <script defer src="script.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #222;
            color: white;
            padding: 20px;
        }
        .timeline-container, .arguments-container, .impact-container {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 20px;
        }
        .timeline-item, button {
            padding: 10px 20px;
            background-color: #007BFF;
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        .timeline-item:hover, button:hover {
            background-color: #0056b3;
        }
        #event-details, #argument-details, #impact-details, #quiz-container {
            margin-top: 20px;
            padding: 15px;
            background-color: white;
            border-radius: 5px;
            display: none;
        }
    </style>
</head>
<body>
    <header>
        <h1>ISRA vs. Chapter 25 Bar and Restaurant</h1>
        <p>An Interactive Legal Presentation</p>
    </header>

    <section id="timeline">
        <h2>Case Timeline</h2>
        <div class="timeline-container">
            <div class="timeline-item" onclick="showDetails('event1')">August 2015 - Case Filed</div>
            <div class="timeline-item" onclick="showDetails('event2')">September 2015 - Interim Injunction</div>
            <div class="timeline-item" onclick="showDetails('event3')">August 2016 - Final Judgment</div>
        </div>
        <div id="event-details"></div>
    </section>

    <section id="arguments">
        <h2>Argument Battles</h2>
        <button onclick="showArguments('isra')">ISRA's Arguments</button>
        <button onclick="showArguments('chapter25')">Chapter 25’s Arguments</button>
        <div id="argument-details"></div>
    </section>

    <section id="impact">
        <h2>Impact & Legacy</h2>
        <button onclick="showImpact('legal')">Legal Precedents</button>
        <button onclick="showImpact('industry')">Impact on Music Industry</button>
        <div id="impact-details"></div>
    </section>

    <section id="quiz">
        <h2>Legal Quiz</h2>
        <p>Test your knowledge of the case!</p>
        <button onclick="startQuiz()">Start Quiz</button>
        <div id="quiz-container"></div>
    </section>

    <footer>
        <p>Copyright &copy; 2025 - Interactive Legal Presentation</p>
    </footer>

    <script>
        function showDetails(event) {
            let details = {
                'event1': 'In August 2015, ISRA filed the lawsuit against Chapter 25 Bar for playing music without proper licensing.',
                'event2': 'In September 2015, the court granted an interim injunction, restraining the defendant from playing ISRA’s content.',
                'event3': 'In August 2016, the Delhi High Court ruled in favor of ISRA, issuing a permanent injunction and ordering financial disclosures.'
            };
            document.getElementById('event-details').innerHTML = details[event];
            document.getElementById('event-details').style.display = 'block';
        }
        function showArguments(side) {
            let arguments = {
                'isra': 'ISRA argued that performers have a statutory right to royalties under Section 38A and that Chapter 25 Bar failed to obtain a proper license.',
                'chapter25': 'The defendant could have argued that playing background music was incidental and did not qualify as commercial exploitation.'
            };
            document.getElementById('argument-details').innerHTML = arguments[side];
            document.getElementById('argument-details').style.display = 'block';
        }
        function showImpact(type) {
            let impact = {
                'legal': 'This case reinforced the importance of licensing music in commercial establishments and set a precedent for performer rights enforcement.',
                'industry': 'Following this ruling, businesses became more aware of the necessity of paying royalties, leading to stricter compliance with copyright laws.'
            };
            document.getElementById('impact-details').innerHTML = impact[type];
            document.getElementById('impact-details').style.display = 'block';
        }
        function startQuiz() {
            let question = prompt('What section of the Copyright Act, 1957 protects performers’ rights? (A) 18, (B) 38A, (C) 52, (D) 65');
            alert(question.toUpperCase() === 'B' ? 'Correct!' : 'Try Again!');
        }
    </script>
</body>
</html>
