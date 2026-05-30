<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>QR Tab Filler</title>
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link href="https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=Syne:wght@400;600;800&display=swap" rel="stylesheet" />
<script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>

<style>
  /* ── RESET & BASE ─────────────────────────────────────────────────── */
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --bg:        #0b0c10;
    --surface:   #12141a;
    --card:      #181b24;
    --border:    #252836;
    --accent:    #e8ff47;
    --accent2:   #47ffe8;
    --danger:    #ff4747;
    --text:      #e8eaf0;
    --muted:     #5a5f72;
    --radius:    10px;
    --mono:      'Space Mono', monospace;
    --sans:      'Syne', sans-serif;
  }

  html, body {
    min-height: 100%;
    background: var(--bg);
    color: var(--text);
    font-family: var(--sans);
    -webkit-font-smoothing: antialiased;
  }

  body {
    background-image:
      radial-gradient(ellipse 60% 40% at 80% 10%, rgba(232,255,71,.07) 0%, transparent 60%),
      radial-gradient(ellipse 50% 60% at 10% 90%, rgba(71,255,232,.05) 0%, transparent 55%);
    min-height: 100vh;
  }

  /* ── LAYOUT ────────────────────────────────────────────────────────── */
  .shell {
    max-width: 860px;
    margin: 0 auto;
    padding: 40px 20px 80px;
  }

  /* ── HEADER ────────────────────────────────────────────────────────── */
  header {
    display: flex;
    align-items: flex-end;
    justify-content: space-between;
    margin-bottom: 44px;
    gap: 16px;
    flex-wrap: wrap;
  }

  .logo-block {}
  .logo-tag {
    font-family: var(--mono);
    font-size: 10px;
    letter-spacing: .2em;
    color: var(--accent);
    text-transform: uppercase;
    margin-bottom: 6px;
  }
  h1 {
    font-size: clamp(28px, 5vw, 44px);
    font-weight: 800;
    line-height: 1;
    letter-spacing: -.02em;
    color: var(--text);
  }
  h1 span { color: var(--accent); }

  .header-stats {
    display: flex;
    gap: 20px;
    align-items: center;
  }
  .stat-pill {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 100px;
    padding: 6px 16px;
    font-family: var(--mono);
    font-size: 12px;
    color: var(--muted);
  }
  .stat-pill strong { color: var(--accent); }

  /* ── FORM CARD ─────────────────────────────────────────────────────── */
  .form-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 28px 28px 24px;
    margin-bottom: 36px;
    position: relative;
    overflow: hidden;
  }
  .form-card::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 2px;
    background: linear-gradient(90deg, var(--accent), var(--accent2));
  }

  .form-title {
    font-size: 13px;
    font-family: var(--mono);
    letter-spacing: .15em;
    color: var(--muted);
    text-transform: uppercase;
    margin-bottom: 20px;
  }

  .fields {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 12px;
    margin-bottom: 16px;
  }
  @media (max-width: 600px) { .fields { grid-template-columns: 1fr; } }

  label {
    display: block;
    font-size: 10px;
    font-family: var(--mono);
    letter-spacing: .15em;
    color: var(--muted);
    text-transform: uppercase;
    margin-bottom: 7px;
  }

  input[type="text"] {
    width: 100%;
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 6px;
    color: var(--text);
    font-family: var(--mono);
    font-size: 13px;
    padding: 10px 14px;
    outline: none;
    transition: border-color .2s, box-shadow .2s;
  }
  input[type="text"]:focus {
    border-color: var(--accent);
    box-shadow: 0 0 0 3px rgba(232,255,71,.12);
  }
  input[type="text"]::placeholder { color: var(--muted); }

  .form-actions {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
  }

  /* ── BUTTONS ───────────────────────────────────────────────────────── */
  .btn {
    display: inline-flex;
    align-items: center;
    gap: 7px;
    font-family: var(--mono);
    font-size: 12px;
    font-weight: 700;
    letter-spacing: .08em;
    text-transform: uppercase;
    border: none;
    border-radius: 6px;
    cursor: pointer;
    padding: 10px 20px;
    transition: transform .15s, opacity .15s, box-shadow .15s;
    user-select: none;
  }
  .btn:active { transform: scale(.97); }

  .btn-primary {
    background: var(--accent);
    color: #0b0c10;
  }
  .btn-primary:hover { box-shadow: 0 0 18px rgba(232,255,71,.35); }

  .btn-ghost {
    background: transparent;
    border: 1px solid var(--border);
    color: var(--muted);
  }
  .btn-ghost:hover { border-color: var(--muted); color: var(--text); }

  .btn-danger {
    background: transparent;
    border: 1px solid rgba(255,71,71,.3);
    color: var(--danger);
  }
  .btn-danger:hover { background: rgba(255,71,71,.08); border-color: var(--danger); }

  .btn-sm {
    padding: 6px 12px;
    font-size: 10px;
  }

  /* ── SECTION HEADER ────────────────────────────────────────────────── */
  .section-head {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 18px;
  }
  .section-title {
    font-size: 11px;
    font-family: var(--mono);
    letter-spacing: .2em;
    color: var(--muted);
    text-transform: uppercase;
  }

  /* ── GRID & CARDS ──────────────────────────────────────────────────── */
  #grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(230px, 1fr));
    gap: 18px;
  }

  .qr-card {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    animation: fadeUp .3s ease both;
    transition: border-color .2s, transform .2s, box-shadow .2s;
  }
  .qr-card:hover {
    border-color: rgba(232,255,71,.25);
    transform: translateY(-3px);
    box-shadow: 0 12px 32px rgba(0,0,0,.4);
  }

  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(14px); }
    to   { opacity: 1; transform: translateY(0);    }
  }

  .qr-img-wrap {
    background: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 16px;
  }
  .qr-img-wrap canvas,
  .qr-img-wrap img { display: block; width: 100% !important; height: auto !important; }

  .qr-body {
    padding: 14px 16px;
    flex: 1;
    display: flex;
    flex-direction: column;
    gap: 6px;
  }

  .qr-name {
    font-size: 14px;
    font-weight: 600;
    color: var(--text);
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }

  .qr-val {
    font-family: var(--mono);
    font-size: 10px;
    color: var(--muted);
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .qr-val span { color: var(--accent2); }

  .qr-date {
    font-family: var(--mono);
    font-size: 9px;
    color: #3a3e50;
    margin-top: 2px;
  }

  .qr-footer {
    padding: 10px 16px 14px;
    display: flex;
    gap: 8px;
  }

  /* ── EMPTY STATE ───────────────────────────────────────────────────── */
  #empty {
    text-align: center;
    padding: 60px 20px;
    display: none;
  }
  #empty.visible { display: block; }

  .empty-icon {
    font-size: 48px;
    margin-bottom: 16px;
    opacity: .4;
  }
  .empty-label {
    font-family: var(--mono);
    font-size: 12px;
    letter-spacing: .15em;
    color: var(--muted);
    text-transform: uppercase;
  }

  /* ── TOAST ─────────────────────────────────────────────────────────── */
  #toast {
    position: fixed;
    bottom: 28px; left: 50%; transform: translateX(-50%) translateY(20px);
    background: var(--accent);
    color: #0b0c10;
    font-family: var(--mono);
    font-size: 12px;
    font-weight: 700;
    letter-spacing: .08em;
    text-transform: uppercase;
    padding: 10px 24px;
    border-radius: 100px;
    opacity: 0;
    pointer-events: none;
    transition: opacity .25s, transform .25s;
    z-index: 999;
    white-space: nowrap;
  }
  #toast.show { opacity: 1; transform: translateX(-50%) translateY(0); }

  /* ── MODAL ─────────────────────────────────────────────────────────── */
  .modal-overlay {
    position: fixed; inset: 0;
    background: rgba(0,0,0,.65);
    display: flex; align-items: center; justify-content: center;
    z-index: 200;
    opacity: 0; pointer-events: none;
    transition: opacity .2s;
    backdrop-filter: blur(4px);
  }
  .modal-overlay.open { opacity: 1; pointer-events: all; }

  .modal {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 32px 28px 24px;
    max-width: 380px;
    width: 90%;
    transform: scale(.95) translateY(10px);
    transition: transform .2s;
  }
  .modal-overlay.open .modal { transform: scale(1) translateY(0); }

  .modal h2 {
    font-size: 18px;
    font-weight: 800;
    margin-bottom: 8px;
  }
  .modal p {
    font-size: 13px;
    color: var(--muted);
    line-height: 1.6;
    margin-bottom: 24px;
  }
  .modal-actions { display: flex; gap: 10px; justify-content: flex-end; }

  /* ── SCROLLBAR ─────────────────────────────────────────────────────── */
  ::-webkit-scrollbar { width: 6px; }
  ::-webkit-scrollbar-track { background: var(--bg); }
  ::-webkit-scrollbar-thumb { background: var(--border); border-radius: 3px; }
</style>
</head>
<body>

<div class="shell">

  <!-- HEADER -->
  <header>
    <div class="logo-block">
      <div class="logo-tag">// QR Tab Filler v2.0</div>
      <h1>QR <span>Store</span></h1>
    </div>
    <div class="header-stats">
      <div class="stat-pill">Total: <strong id="stat-count">0</strong></div>
      <button class="btn btn-danger btn-sm" onclick="confirmReset()">↺ Reset</button>
    </div>
  </header>

  <!-- FORM -->
  <div class="form-card">
    <div class="form-title">// Tambah QR Baru</div>
    <div class="fields">
      <div>
        <label for="f-nama">Nama / Label</label>
        <input type="text" id="f-nama" placeholder="Login-Admin" />
      </div>
      <div>
        <label for="f-k1">Kolom 1</label>
        <input type="text" id="f-k1" placeholder="Username / NIP" />
      </div>
      <div>
        <label for="f-k2">Kolom 2</label>
        <input type="text" id="f-k2" placeholder="Password" />
      </div>
    </div>
    <div class="form-actions">
      <button class="btn btn-primary" onclick="addQR()">
        <span>+</span> Generate &amp; Simpan
      </button>
      <button class="btn btn-ghost" onclick="clearForm()">Bersihkan</button>
    </div>
  </div>

  <!-- LIST -->
  <div class="section-head">
    <div class="section-title">// QR Tersimpan</div>
  </div>

  <div id="empty">
    <div class="empty-icon">⬛</div>
    <div class="empty-label">Belum ada QR tersimpan</div>
  </div>

  <div id="grid"></div>

</div><!-- /shell -->

<!-- TOAST -->
<div id="toast"></div>

<!-- MODAL KONFIRMASI RESET -->
<div class="modal-overlay" id="modal-reset">
  <div class="modal">
    <h2>Reset semua QR?</h2>
    <p>Semua data QR yang tersimpan akan dihapus permanen.<br>Tindakan ini tidak dapat dibatalkan.</p>
    <div class="modal-actions">
      <button class="btn btn-ghost" onclick="closeModal()">Batal</button>
      <button class="btn btn-danger" onclick="resetAll()">Ya, Hapus Semua</button>
    </div>
  </div>
</div>

<!-- MODAL KONFIRMASI HAPUS SATU -->
<div class="modal-overlay" id="modal-del">
  <div class="modal">
    <h2>Hapus QR ini?</h2>
    <p id="modal-del-label">QR "<strong></strong>" akan dihapus.</p>
    <div class="modal-actions">
      <button class="btn btn-ghost" onclick="closeModal()">Batal</button>
      <button class="btn btn-danger" onclick="confirmDelete()">Hapus</button>
    </div>
  </div>
</div>

<script>
// ── STORAGE KEY ─────────────────────────────────────────────────────────────
const LS_KEY = 'qr_tab_filler_v2';

// ── DB (localStorage) ────────────────────────────────────────────────────────
function loadDB() {
  try { return JSON.parse(localStorage.getItem(LS_KEY)) || []; }
  catch { return []; }
}
function saveDB(list) {
  localStorage.setItem(LS_KEY, JSON.stringify(list));
}
function genId() {
  return Math.random().toString(36).slice(2, 8).toUpperCase();
}

// ── STATE ────────────────────────────────────────────────────────────────────
let pendingDeleteId = null;

// ── TOAST ────────────────────────────────────────────────────────────────────
let toastTimer;
function showToast(msg) {
  const t = document.getElementById('toast');
  t.textContent = msg;
  t.classList.add('show');
  clearTimeout(toastTimer);
  toastTimer = setTimeout(() => t.classList.remove('show'), 2200);
}

// ── MODAL ────────────────────────────────────────────────────────────────────
function confirmReset() {
  document.getElementById('modal-reset').classList.add('open');
}
function confirmDeleteModal(id) {
  const list = loadDB();
  const item = list.find(q => q.id === id);
  if (!item) return;
  pendingDeleteId = id;
  document.getElementById('modal-del-label').innerHTML =
    `QR "<strong>${escHtml(item.nama)}</strong>" akan dihapus.`;
  document.getElementById('modal-del').classList.add('open');
}
function closeModal() {
  document.querySelectorAll('.modal-overlay').forEach(m => m.classList.remove('open'));
  pendingDeleteId = null;
}
// Close on backdrop click
document.querySelectorAll('.modal-overlay').forEach(overlay => {
  overlay.addEventListener('click', e => { if (e.target === overlay) closeModal(); });
});

// ── RESET ALL ────────────────────────────────────────────────────────────────
function resetAll() {
  localStorage.removeItem(LS_KEY);
  closeModal();
  renderGrid();
  showToast('Semua QR dihapus');
}

// ── DELETE ONE ───────────────────────────────────────────────────────────────
function confirmDelete() {
  if (!pendingDeleteId) return;
  let list = loadDB();
  list = list.filter(q => q.id !== pendingDeleteId);
  saveDB(list);
  closeModal();
  renderGrid();
  showToast('QR dihapus');
}

// ── ESCAPE HTML ──────────────────────────────────────────────────────────────
function escHtml(s) {
  return String(s)
    .replace(/&/g,'&amp;').replace(/</g,'&lt;')
    .replace(/>/g,'&gt;').replace(/"/g,'&quot;');
}

// ── FORMAT DATE ──────────────────────────────────────────────────────────────
function fmtDate(iso) {
  try {
    return new Date(iso).toLocaleString('id-ID', {
      day:'2-digit', month:'short', year:'numeric',
      hour:'2-digit', minute:'2-digit'
    });
  } catch { return iso; }
}

// ── GENERATE QR INTO ELEMENT ──────────────────────────────────────────────────
function makeQRElement(wrap, k1, k2) {
  wrap.innerHTML = '';
  // QRCode lib requires a container div
  new QRCode(wrap, {
    text: k1 + '\t' + k2,
    width: 200,
    height: 200,
    colorDark: '#1a1a2e',
    colorLight: '#ffffff',
    correctLevel: QRCode.CorrectLevel.M,
  });
}

// ── DOWNLOAD QR ──────────────────────────────────────────────────────────────
function downloadQR(id) {
  const wrap = document.querySelector(`[data-qr-wrap="${id}"]`);
  if (!wrap) return;
  const canvas = wrap.querySelector('canvas');
  const img    = wrap.querySelector('img');
  let src;
  if (canvas) {
    src = canvas.toDataURL('image/png');
  } else if (img) {
    src = img.src;
  } else { return; }

  const list = loadDB();
  const item = list.find(q => q.id === id);
  const name = item ? item.nama.replace(/[^a-zA-Z0-9_-]/g,'_') : 'qr';

  const a = document.createElement('a');
  a.href = src;
  a.download = `QR_${name}.png`;
  a.click();
  showToast('QR diunduh');
}

// ── RENDER GRID ───────────────────────────────────────────────────────────────
function renderGrid() {
  const list  = loadDB();
  const grid  = document.getElementById('grid');
  const empty = document.getElementById('empty');
  document.getElementById('stat-count').textContent = list.length;

  grid.innerHTML = '';

  if (list.length === 0) {
    empty.classList.add('visible');
    return;
  }
  empty.classList.remove('visible');

  list.forEach((item, idx) => {
    const card = document.createElement('div');
    card.className = 'qr-card';
    card.style.animationDelay = (idx * 50) + 'ms';

    card.innerHTML = `
      <div class="qr-img-wrap" data-qr-wrap="${escHtml(item.id)}"></div>
      <div class="qr-body">
        <div class="qr-name" title="${escHtml(item.nama)}">${escHtml(item.nama)}</div>
        <div class="qr-val"><span>K1</span> ${escHtml(item.kolom1)}</div>
        <div class="qr-val"><span>K2</span> ${escHtml(item.kolom2)}</div>
        <div class="qr-date">${fmtDate(item.createdAt)}</div>
      </div>
      <div class="qr-footer">
        <button class="btn btn-ghost btn-sm" style="flex:1" onclick="downloadQR('${escHtml(item.id)}')">↓ Unduh</button>
        <button class="btn btn-danger btn-sm" onclick="confirmDeleteModal('${escHtml(item.id)}')">✕</button>
      </div>
    `;

    grid.appendChild(card);

    // Generate QR after DOM insert
    const wrap = card.querySelector(`[data-qr-wrap]`);
    makeQRElement(wrap, item.kolom1, item.kolom2);
  });
}

// ── ADD QR ────────────────────────────────────────────────────────────────────
function addQR() {
  const nama  = document.getElementById('f-nama').value.trim();
  const kolom1 = document.getElementById('f-k1').value.trim();
  const kolom2 = document.getElementById('f-k2').value.trim();

  if (!nama)   { flashInput('f-nama',  'Nama wajib diisi'); return; }
  if (!kolom1) { flashInput('f-k1',    'Kolom 1 wajib diisi'); return; }
  if (!kolom2) { flashInput('f-k2',    'Kolom 2 wajib diisi'); return; }

  const list = loadDB();
  list.unshift({
    id: genId(),
    nama,
    kolom1,
    kolom2,
    createdAt: new Date().toISOString(),
  });
  saveDB(list);
  clearForm();
  renderGrid();
  showToast('✓ QR berhasil disimpan');
}

function flashInput(id, msg) {
  const el = document.getElementById(id);
  el.style.borderColor = 'var(--danger)';
  el.style.boxShadow   = '0 0 0 3px rgba(255,71,71,.15)';
  el.placeholder = msg;
  setTimeout(() => {
    el.style.borderColor = '';
    el.style.boxShadow   = '';
    el.placeholder = '';
  }, 1800);
}

function clearForm() {
  document.getElementById('f-nama').value  = '';
  document.getElementById('f-k1').value    = '';
  document.getElementById('f-k2').value    = '';
}

// ── ENTER KEY ────────────────────────────────────────────────────────────────
['f-nama','f-k1','f-k2'].forEach(id => {
  document.getElementById(id).addEventListener('keydown', e => {
    if (e.key === 'Enter') addQR();
  });
});

// ── INIT ──────────────────────────────────────────────────────────────────────
renderGrid();
</script>
</body>
</html>
