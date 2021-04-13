# Chart.js , Canvas

**Chart.js is an open source library in Javascript that will help us drawing charts in order to represent data in more appropriate and readable way with visual drawings. It's also well documented and easy to create and represent.**

**There are many ways that we can use to include Chart.js in our project either by downloading the files and including it in the project files but there is a better and easier way of doing this by using cdn (Content Delivery Network). and in this read I will explain how to use cdn to include the library in any website.**

**Code needed in HTML file:**

```html
<body>
    <canvas id="sales" width="500" height="500"></canvas>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
</body>

```

**Javascript code:**

```javascript
//this code was copied directly for chart.js website
let ctx = document.getElementById('sales').getContext('2d');
let myChart = new Chart(ctx, {
    type: 'bar',
    data: {
        labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
        datasets: [{
            label: 'Sales data',
            data: [12, 19, 3, 5, 2, 3],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)',
            ],
            borderWidth: 1
        }]
    },
    options: {
        scales: {
            y: {
                beginAtZero: true
            }
        }
    }
});

```
**We can also change the style of the chart with ease from the javascript code like above.** 