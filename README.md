:root {
  font-family: Inter, Arial, sans-serif;
  color: #f5f5f5;
  background: #0b0b10;
}

* { box-sizing: border-box; }

body {
  margin: 0;
  min-width: 320px;
  background:
    radial-gradient(circle at top left, rgba(180, 90, 255, 0.22), transparent 25%),
    radial-gradient(circle at top right, rgba(255, 80, 160, 0.18), transparent 25%),
    #0b0b10;
}

.page {
  max-width: 1150px;
  margin: 0 auto;
  padding: 24px;
}

.hero,
.card,
.lead {
  background: rgba(255,255,255,0.05);
  border: 1px solid rgba(255,255,255,0.08);
  border-radius: 20px;
}

.hero {
  display: flex;
  justify-content: space-between;
  gap: 20px;
  align-items: center;
  padding: 24px;
  margin-bottom: 24px;
}

.eyebrow {
  text-transform: uppercase;
  letter-spacing: 0.12em;
  color: #d3a9ff;
  font-size: 0.8rem;
}

.hero h1 {
  margin: 0 0 8px;
  font-size: 2.2rem;
}

.sub {
  margin: 0;
  color: #d7d7e0;
}

.grid {
  display: grid;
  grid-template-columns: 360px 1fr;
  gap: 24px;
}

.card {
  padding: 20px;
}

.card h2 {
  margin-top: 0;
}

label {
  display: block;
  margin-bottom: 12px;
  color: #d7d7e0;
  font-size: 0.95rem;
}

input {
  width: 100%;
  margin-top: 6px;
  border-radius: 12px;
  border: 1px solid rgba(255,255,255,0.12);
  background: rgba(255,255,255,0.04);
  color: white;
  padding: 12px 14px;
}

button {
  border: 0;
  border-radius: 12px;
  padding: 12px 16px;
  cursor: pointer;
  font-weight: 700;
  background: linear-gradient(90deg, #ff4fb3, #9b5cff);
  color: white;
}

button:disabled {
  opacity: 0.6;
  cursor: not-allowed;
}

.message {
  color: #e9c9ff;
  margin-top: 12px;
}

.lead-list {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.lead {
  padding: 16px;
  display: flex;
  justify-content: space-between;
  gap: 16px;
  align-items: center;
}

.lead p {
  margin: 6px 0 0;
  color: #cfcfe0;
}

.lead-right {
  display: flex;
  flex-direction: column;
  gap: 10px;
  align-items: flex-end;
}

.badge {
  border-radius: 999px;
  padding: 6px 10px;
  font-size: 0.82rem;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  background: rgba(255,255,255,0.08);
}

.badge.new {
  background: rgba(100, 149, 255, 0.22);
}

.badge.queued {
  background: rgba(100, 255, 170, 0.2);
}

@media (max-width: 900px) {
  .grid {
    grid-template-columns: 1fr;
  }

  .hero {
    flex-direction: column;
    align-items: flex-start;
  }
}
