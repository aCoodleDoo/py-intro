---
layout: two-cols
---

# Meet Your Shadow

<div class="agent-container">
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
.agent-container {
  position: relative;
  width: 100%;
  height: 90%;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
}

.interactive-map {
  width: 100%;
  height: 100%;
  border: none;
  transition: filter 0.3s ease;
  /* Isolate iframe from parent styling */
  color-scheme: light;
  background: white;
}
</style>



::right::


<div class="space-y-6" v-click>

## The Old Way
- Filling out long, confusing forms
- Forgetting important information
- Feeling overwhelmed and impersonal

</div>

<div class="space-y-6" v-click>

## The New Way
- A simple, guided conversation
- The AI asks for information as needed
- A more human-centered experience

</div>

<div class="space-y-6" v-click>

## Holds Your Hand
- Acts as your helpful guide
- Answers common questions
- Shows a clear path to completion

</div>