---
layout: two-cols
layoutClass: gap-16
transition: fade-out
---

# Intro

Computer programs consist of commands

and each command instructing the computer to take some action.

A computer executes these commands one by one.

commands can be used to:

<v-clicks>

- post messages or ask for info from the user.
- perform calculations on numbers.
- compare things in the computer's memory.
- cause changes in how the program functions.

</v-clicks>

::right::

<div class="app-container">
  <a 
    href="https://v0-property-maintenance-app-one.vercel.app/tenant"
    target="_blank"
    rel="noopener noreferrer"
    class="interactive-app-link"
  >
    <div class="link-content">
      <h3>🏠 Try the Tenant Portal</h3>
      <p>Click to open Property Management Demo</p>
      <span class="external-link-icon">↗</span>
    </div>
  </a>
</div>

<style scoped>
.app-container {
  position: relative;
  width: 90%;
  height: 80%;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
  border: 2px solid #e5e7eb;
}

.interactive-app-link {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
  text-decoration: none;
  color: inherit;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  transition: all 0.3s ease;
  position: relative;
}

.interactive-app-link:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
}

.link-content {
  text-align: center;
  color: white;
}

.link-content h3 {
  margin: 0 0 8px 0;
  font-size: 1.5rem;
  font-weight: 600;
}

.link-content p {
  margin: 0;
  opacity: 0.9;
  font-size: 1rem;
}

.external-link-icon {
  position: absolute;
  top: 10px;
  right: 10px;
  font-size: 1.2rem;
  opacity: 0.8;
}
</style>
