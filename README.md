# Chart.js
My self learning on Chart.js

![image](https://user-images.githubusercontent.com/56244402/110635015-3ad93100-81dd-11eb-947f-26989fdfde5e.png)

## Getting Started

Let's get started using Chart.js!

First, we need to have a canvas in our page.
```
<canvas id="myChart"></canvas>
```
Now that we have a canvas we can use, we need to include Chart.min.js & jquery.min.js in our page.

```
<script type="text/javascript" src="js/jquery.min.js"></script>
<script type="text/javascript" src="js/Chart.min.js"></script>
```
Now, we can create a chart. We add a script to our page:

```
var ctx = document.getElementById('myChart').getContext('2d');
var chart = new Chart(ctx, {
    // The type of chart we want to create
    type: 'bar',

    // The data for our dataset
    data: {
        labels: ['January', 'February', 'March', 'April', 'May', 'June', 'July'],
        datasets: [{
            label: 'My First dataset',
            backgroundColor: 'rgb(255, 99, 132)',
            borderColor: 'rgb(255, 99, 132)',
            data: [0, 10, 5, 2, 20, 30, 45]
        }]
    },

    // Configuration options go here
    options: {}
});
```
Test on sample.html
