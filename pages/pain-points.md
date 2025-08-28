---
layout: two-cols
---

# Current Pain Points

<div class="map-container">
  <iframe 
    src="https://www.openstreetmap.org/export/embed.html?bbox=-87.9401,41.6445,-87.5245,42.0230&layer=mapnik&marker=41.8781,-87.6298"
    class="interactive-map"
    frameborder="0"
    scrolling="no"
    marginheight="0"
    marginwidth="0"
    loading="lazy"
    title="Chicago Property Management Area"
  >
  </iframe>
  <div class="map-overlay">
    <div class="location-marker">📍 Chicago, IL</div>
  </div>
</div>

<style scoped>
.map-container {
  position: relative;
  width: 100%;
  height: 75%;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
}

.interactive-map {
  width: 100%;
  height: 75%;
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

::right::

<div class="space-y-6" v-click>

## Documentation Burden
- Field workers avoid paperwork
- Manual photo management
- Repetitive form filling

</div>

<div class="space-y-6" v-click>

## Communication Friction
- Multiple stakeholder coordination
- Information lost in translation
- Delayed response cycles

</div>

<div class="space-y-6" v-click>

## Administrative Overhead
- Duplicate data entry
- Complex software training
- Manual report generation

</div>



