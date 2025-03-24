<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ISRA vs. Chapter 25 Bar - Case Analysis</title>
    <link rel="stylesheet" href="styles.css">
    <script defer src="script.js"></script>
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
</body>
</html>
