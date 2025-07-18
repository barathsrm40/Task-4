# Task-4
{
  "manifest_version": 3,
  "name": "TimeTrackPro",
  "version": "1.0",
  "description": "Track time and productivity analytics",
  "permissions": ["tabs", "storage", "activeTab", "scripting"],
  "background": {
    "service_worker": "background.js"
  },
  "action": {
    "default_popup": "popup.html"
  }
}

const ctx = document.getElementById('productivityChart');
new Chart(ctx, {
  type: 'doughnut',
  data: {
    labels: ['Productive', 'Unproductive'],
    datasets: [{
      data: [60, 40],  // Fetched from backend
      backgroundColor: ['green', 'red']
    }]
  }
});
{
  "userId": "user123",
  "website": "youtube.com",
  "duration": 360,  // in seconds
  "productive": false,
  "date": "2025-07-17"
}
Week Summary:
- Total Time: 10 hrs
- Productive: 6 hrs (60%)
- Unproductive: 4 hrs (40%)
