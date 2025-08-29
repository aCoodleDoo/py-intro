---
layout: two-cols
---

# Current Pain Points

<div class="map-container">
  <iframe 
    src="https://app.powerbi.com/view?r=eyJrIjoiYjE1OTJkMjItZDFkZi00YjhjLTkwN2MtODU1N2ZmNDE5OTEyIiwidCI6ImJmNDlkMzdjLTE0YWQtNDU0MS1iNDA1LTQxOWZlM2Q1NjYzYSJ9"
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
    <div class="location-marker">📍 Raleigh, NC</div>
  </div>
</div>

<style scoped>
.map-container {
  position: relative;
  width: 90%;
  height: 60%;
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

::right::

<div class="space-y-6" v-click>

## Documentation Burden
- We avoid paperwork
- We like to talk and take pictures
- Good documentation is valuable

</div>

<div class="space-y-6" v-click>

## Communication Friction
- Multiple stakeholders to coordinate
- Miscommunication due to information overload
- Delayed simple responses

</div>

<div class="space-y-6" v-click>

## Admin Overhead
- Duplicate data entry
- Complex software training
- Manual report generation

</div>



