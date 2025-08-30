
---
layout: center
---

# Patient Care Coordinator AI Agent

<div class="agent-container">
  <iframe 
    id="JotFormIFrame-019761564a40774fb9e0437c063b514ea274"
    title="Patient Care Coordinator AI Agent" 
    onload="window.parent.scrollTo(0,0)"
    allowtransparency="true" 
    allow="geolocation; microphone; camera; fullscreen"
    src="https://agent.jotform.com/019761564a40774fb9e0437c063b514ea274?embedMode=iframe&background=1&shadow=1"
    frameborder="0" 
    style="max-width:100%; height:688px; border:none; width:100%;" 
    scrolling="no"
    class="interactive-agent">
  </iframe>
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
.agent-container {
  position: relative;
  width: 90%;
  height: 80vh;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
  margin: 0 auto;
}

.interactive-agent {
  width: 100%;
  height: 100%;
  border: none;
  transition: filter 0.3s ease;
}

.agent-container:hover .interactive-agent {
  filter: brightness(1.05);
}
</style>
