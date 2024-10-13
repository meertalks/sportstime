document.addEventListener('DOMContentLoaded', function () {
    const scoreContainer = document.getElementById('score-container');

    // Replace 'YOUR_API_KEY' with your actual CricAPI key
    const apiKey = 'YOUR_API_KEY';
    const apiUrl = `https://cricapi.com/api/matches?apikey=${apiKey}`;

    async function fetchLiveScores() {
        try {
            const response = await fetch(apiUrl);
            const data = await response.json();
            displayScores(data.matches);
        } catch (error) {
            console.error('Error fetching live scores:', error);
            scoreContainer.innerHTML = `<p>Unable to fetch live scores at this moment.</p>`;
        }
    }

    function displayScores(matches) {
        scoreContainer.innerHTML = ''; // Clear existing content

        // Filter live matches
        const liveMatches = matches.filter(match => match.matchStarted && match.live);

        if (liveMatches.length === 0) {
            scoreContainer.innerHTML = `<p>No live matches at the moment.</p>`;
            return;
        }

        // Loop through each live match and display the score
        liveMatches.forEach(match => {
            const matchElement = document.createElement('div');
            matchElement.classList.add('match');

            matchElement.innerHTML = `
                <h3>${match['team-1']} vs ${match['team-2']}</h3>
                <p><strong>Status:</strong> ${match.matchStarted ? 'Live' : 'Upcoming'}</p>
                <p><strong>Score:</strong> ${match.score || 'Not available yet'}</p>
            `;

            scoreContainer.appendChild(matchElement);
        });
    }

    fetchLiveScores(); // Fetch the scores on page load
});
