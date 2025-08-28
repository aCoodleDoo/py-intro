
---
layout: two-cols
---

# Analytics

<script setup>
import { onMounted, ref } from 'vue'
import { Chart, registerables } from 'chart.js'

Chart.register(...registerables)

const chartRef = ref(null)

onMounted(() => {
  const ctx = chartRef.value.getContext('2d')
  new Chart(ctx, {
    type: 'line',
    data: {
      labels: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun'],
      datasets: [{
        label: 'User Growth',
        data: [12, 19, 15, 25, 32, 45],
        borderColor: '#3b82f6',
        backgroundColor: 'rgba(59, 130, 246, 0.1)',
        borderWidth: 3,
        fill: true,
        tension: 0.4
      }, {
        label: 'Revenue ($K)',
        data: [8, 15, 12, 20, 28, 38],
        borderColor: '#10b981',
        backgroundColor: 'rgba(16, 185, 129, 0.1)',
        borderWidth: 3,
        fill: true,
        tension: 0.4
      }]
    },
    options: {
      responsive: true,
      maintainAspectRatio: false,
      plugins: {
        legend: {
          position: 'top',
        }
      },
      scales: {
        y: {
          beginAtZero: true,
          grid: {
            color: 'rgba(0, 0, 0, 0.1)'
          }
        },
        x: {
          grid: {
            color: 'rgba(0, 0, 0, 0.1)'
          }
        }
      }
    }
  })
})
</script>

<div class="chart-container" v-click>
  <canvas ref="chartRef" width="400" height="200"></canvas>
</div>

<style scoped>
.chart-container {
  width: 100%;
  height: 300px;
  margin: 20px 0;
  padding: 20px;
  background: white;
  border-radius: 8px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}
</style>

::right::

<div class="space-y-6" v-click>

## Strategic Advantage
- First-mover market positioning
- 12-18 month competitive edge
- Brand leadership establishment

</div>

<div class="space-y-6" v-click>

## Business Impact
- 90% reduction in administrative work
- Improved tenant satisfaction
- Higher owner retention rates

</div>

<div class="space-y-6" v-click>

## Next Steps
- Schedule product demonstration
- Identify pilot implementation
- Begin strategic planning

</div>
