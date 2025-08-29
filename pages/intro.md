---
layout: two-cols
layoutClass: gap-16
transition: fade-out
---

# Intro

Context collection

A support ticket is a **container** that **collects context**

through a standard form template and collects 

information like:

<v-clicks>

- Contact information (user)
- Date and Location of the issue (property)
- Detailed description of the issue (work order)
- End to End Visibility (company)

</v-clicks>

::right::

<div class="app-container">
  <iframe 
    src="https://v0-property-maintenance-app-one.vercel.app/tenant"
    class="interactive-app"
    frameborder="0"
    scrolling="no"
    marginheight="0"
    marginwidth="0"
    loading="lazy"
    title="Property Maintenance Tenant Portal"
  >
  </iframe>
  <div class="app-overlay">
    <div class="app-label">🏠 Tenant Portal Demo</div>
  </div>
</div>

<style scoped>
.app-container {
  position: relative;
  width: 100%;
  height: 100%;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
}

.interactive-app {
  width: 100%;
  height: 100%;
  border: none;
  transition: filter 0.3s ease;
}

.app-container:hover .interactive-app {
  filter: brightness(1.1);
}

.app-overlay {
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

.app-label {
  display: flex;
  align-items: center;
  gap: 4px;
}
</style>