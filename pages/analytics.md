---
layout: two-cols
---

# Analytics

<script setup>
import { ref, onMounted } from 'vue'
import {
  Chart as ChartJS,
  CategoryScale,
  LinearScale,
  PointElement,
  LineElement,
  Title,
  Tooltip,
  Legend,
  Filler
} from 'chart.js'

ChartJS.register(
  CategoryScale,
  LinearScale,
  PointElement,
  LineElement,
  Title,
  Tooltip,
  Legend,
  Filler
)

const canvasRef = ref(null)

onMounted(() => {
  if (!canvasRef.value) return
  
  const ctx = canvasRef.value.getContext('2d')
  new ChartJS(ctx, {
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

::right::

<div class="chart-container" style="position: relative; height: 400px; width: 100%;">
  <canvas ref="canvasRef"></canvas>
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