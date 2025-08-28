---
layout: two-cols
---

# Analytics

<script setup>
import { ref, onMounted } from 'vue'
import Chart from 'chart.js/auto'

const chartRef = ref(null)

onMounted(() => {
  const ctx = chartRef.value.getContext('2d')
  new Chart(ctx, {
    type: 'line',
    data: {
      labels: ['Pre-Implementation', 'Month 1', 'Month 3', 'Month 6', 'Month 9', 'Month 12'],
      datasets: [{
        label: 'Human Effort (%)',
        data: [100, 85, 65, 45, 30, 20],
        borderColor: '#ef4444',
        backgroundColor: 'rgba(239, 68, 68, 0.1)',
        borderWidth: 3,
        fill: true,
        tension: 0.4
      }, {
        label: 'Agent Effort (%)',
        data: [0, 15, 35, 55, 70, 80],
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
        },
        title: {
          display: true,
          text: 'Automation Implementation Timeline',
          font: {
            size: 16,
            weight: 'bold'
          }
        }
      },
      scales: {
        y: {
          beginAtZero: true,
          max: 100,
          ticks: {
            callback: function(value) {
              return value + '%'
            }
          },
          title: {
            display: true,
            text: 'Effort Distribution'
          },
          grid: {
            color: 'rgba(0, 0, 0, 0.1)'
          }
        },
        x: {
          title: {
            display: true,
            text: 'Implementation Timeline'
          },
          grid: {
            color: 'rgba(0, 0, 0, 0.1)'
          }
        }
      }
    }
  })
})
</script>

::left::

<div class="prose" v-click>

## Analytics

The adoption of automation in business processes has shown a significant shift in effort distribution. Initially, human effort accounts for the entirety of task execution. As automation is progressively implemented, the reliance on human input decreases, while agent (automated system) effort increases proportionally. This transition not only streamlines operations but also allows human resources to focus on more complex, strategic, and creative endeavors, ultimately driving greater business value.

</div>

::right::

<div class="chart-container" ref="chartRef">
  <canvas ref="chartRef"></canvas>
</div>

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