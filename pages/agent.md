---
layout: two-cols
---

# Form = AI Agent

::right::

<div class="map-container">
  <iframe 
    id="JotFormIFrame-019761564a40774fb9e0437c063b514ea274"
    title="Patient Care Coordinator AI Agent" 
    onload="window.parent.scrollTo(0,0)"
    allowtransparency="true" 
    allow="geolocation; microphone; camera; fullscreen"
    src="https://agent.jotform.com/019761564a40774fb9e0437c063b514ea274?embedMode=iframe&background=1&shadow=1"
    frameborder="0" 
    scrolling="no"
    marginheight="0"
    marginwidth="0"
    loading="lazy"
    class="interactive-map"
  >
  </iframe>
  <div class="map-overlay">
    <div class="location-marker">🤖 AI Agent</div>
  </div>
</div>

<script setup>
import { onMounted } from 'vue'

onMounted(() => {
  // Load JotForm embed handler script
  const script = document.createElement('script')
  script.src = 'https://cdn.jotfor.ms/s/umd/latest/for-form-embed-handler.js'
  script.onload = () => {
    // Initialize JotForm embed handler after script loads
    if (window.jotformEmbedHandler) {
      window.jotformEmbedHandler("iframe[id='JotFormIFrame-019761564a40774fb9e0437c063b514ea274']", "https://www.jotform.com")
    }
  }
  document.head.appendChild(script)
})
</script>

<style scoped>
.map-container {
  position: relative;
  width: 100%;
  height: 100%;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
}

.interactive-map {
  width: 100%;
  height: 100%;
  border: none;
  transition: filter 0.3s ease;
}

.map-container:hover .interactive-map {
  filter: brightness(1.1);
}

.map-overlay {
  position: absolute;
  top: 10px;
  left: 10px;
  background: rgba(255, 255, 255, 0.9);
  padding: 8px 12px;
  border-radius: 6px;
  font-size: 14px;
  font-weight: 600;
  color: #374151;
  backdrop-filter: blur(4px);
  border: 1px solid rgba(255, 255, 255, 0.2);
}

.location-marker {
  display: flex;
  align-items: center;
  gap: 4px;
}
</style>
