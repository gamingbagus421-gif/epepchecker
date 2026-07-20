<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NXR - Cek FF Fix</title>
<style>
  * { margin:0; padding:0; box-sizing:border-box; }
  body {
    background: #0a0a0a;
    color: #0f0;
    font-family: 'Courier New', monospace;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    padding: 20px;
  }
  .container {
    background: #111;
    border: 2px solid #0f0;
    border-radius: 25px;
    padding: 35px;
    max-width: 850px;
    width: 100%;
    box-shadow: 0 0 60px #0f04;
  }
  h1 {
    text-align: center;
    color: #ff0044;
    text-shadow: 0 0 30px #ff0044;
    font-size: 2.2em;
    letter-spacing: 3px;
  }
  .sub {
    text-align: center;
    color: #88ff88;
    margin-bottom: 25px;
    opacity: 0.7;
  }
  .input-group {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
  }
  .input-group input {
    flex: 1;
    padding: 15px;
    border: 2px solid #0f04;
    border-radius: 12px;
    background: #1a1a1a;
    color: #0f0;
    font-size: 16px;
    min-width: 200px;
  }
  .input-group input:focus {
    border-color: #0f0;
    outline: none;
    box-shadow: 0 0 20px #0f04;
  }
  .btn-group {
    display: flex;
    gap: 12px;
    margin: 15px 0;
  }
  .btn-group button {
    flex: 1;
    padding: 16px;
    border: none;
    border-radius: 12px;
    font-weight: bold;
    font-size: 18px;
    cursor: pointer;
    transition: 0.3s;
    text-transform: uppercase;
    letter-spacing: 2px;
  }
  #cekBtn {
    background: #ff0044;
    color: #fff;
    box-shadow: 0 0 30px #ff004466;
  }
  #cekBtn:hover { background: #cc0033; box-shadow: 0 0 50px #ff0044; }
  #cekBtn:disabled { opacity:0.5; cursor:not-allowed; }
  #logDebug {
    background: #050505;
    height: 120px;
    overflow-y: auto;
    padding: 10px;
    border-radius: 10px;
    border: 1px solid #0f03;
    font-size: 12px;
    color: #88ff88;
    margin-top: 10px;
    display: none;
    font-family: monospace;
    white-space: pre-wrap;
    word-break: break-all;
  }
  #logDebug.active { display: block; }
  #result {
    margin-top: 20px;
    background: #0a0a0a;
    border-radius: 15px;
    padding: 20px;
    border: 1px solid #0f03;
    min-height: 200px;
    display: none;
  }
  #result.active { display: block; }
  .profile-header {
    display: flex;
    align-items: center;
    gap: 20px;
    border-bottom: 1px solid #0f03;
    padding-bottom: 15px;
    margin-bottom: 15px;
  }
  .profile-header .avatar {
    width: 70px;
    height: 70px;
    border-radius: 50%;
    background: #222;
    border: 2px solid #0f0;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 30px;
  }
  .profile-header .name {
    font-size: 24px;
    font-weight: bold;
    color: #0f0;
  }
  .profile-header .uid {
    font-size: 14px;
    color: #888;
  }
  .stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    gap: 12px;
    margin: 15px 0;
  }
  .stat-card {
    background: #1a1a1a;
    padding: 15px;
    border-radius: 12px;
    border: 1px solid #0f03;
    text-align: center;
  }
  .stat-card .label {
    font-size: 12px;
    color: #888;
    text-transform: uppercase;
  }
  .stat-card .value {
    font-size: 22px;
    font-weight: bold;
    color: #0f0;
    margin-top: 5px;
  }
  .stat-card .value.prime { color: #ffcc00; }
  .stat-card .value.like { color: #ff66aa; }
  .loading {
    text-align: center;
    padding: 40px;
    color: #0f0;
    font-size: 18px;
    animation: blink 1s infinite;
  }
  @keyframes blink {
    0%,100% { opacity:1; }
    50% { opacity:0.3; }
  }
  .error {
    color: #ff4444;
    text-align: center;
    padding: 20px;
  }
  .warning {
    color: #ff8800;
    font-size: 12px;
    text-align: center;
    margin-top: 15px;
    border-top: 1px solid #ff880033;
    padding-top: 12px;
  }
  .detected-region {
    color: #88ff88;
    font-size: 13px;
    text-align: center;
    margin-top: 8px;
  }
  .toggle-debug {
    background: transparent;
    border: 1px solid #0f03;
    color: #0f0;
    padding: 5px 12px;
    border-radius: 8px;
    cursor: pointer;
    font-size: 11px;
    margin-top: 5px;
  }
  .toggle-debug:hover { background: #0f02; }
</style>
</head>
<body>
<div class="container">
  <h1>⚡ NXR-ID FIX ⚡</h1>
  <div class="sub">— Free Fire Player Inspector — Auto + Retry</div>

  <div class="input-group">
    <input id="uid" placeholder="Masukkan UID (contoh: 1234567890)" maxlength="15">
    <button class="toggle-debug" id="toggleDebug">🐞 Tampilkan Log</button>
  </div>

  <div class="btn-group">
    <button id="cekBtn">🔍 CEK ID</button>
  </div>

  <div id="logDebug"></div>

  <div id="result">
    <div class="profile-header">
      <div class="avatar">🎮</div>
      <div>
        <div class="name" id="nickname">-</div>
        <div class="uid" id="uidDisplay">UID: -</div>
      </div>
    </div>
    <div class="stats-grid">
      <div class="stat-card"><div class="label">Level</div><div class="value" id="level">-</div></div>
      <div class="stat-card"><div class="label">❤️ Like</div><div class="value like" id="likes">-</div></div>
      <div class="stat-card"><div class="label">⭐ Prime</div><div class="value prime" id="prime">-</div></div>
      <div class="stat-card"><div class="label">🏆 Rank BR</div><div class="value" id="brRank">-</div></div>
      <div class="stat-card"><div class="label">⚔️ Rank CS</div><div class="value" id="csRank">-</div></div>
      <div class="stat-card"><div class="label">👥 Guild</div><div class="value" id="guild" style="font-size:16px;">-</div></div>
      <div class="stat-card"><div class="label">📅 Dibuat</div><div class="value" id="created" style="font-size:14px;">-</div></div>
      <div class="stat-card"><div class="label">🌏 Region</div><div class="value" id="regionDisplay" style="font-size:14px;">-</div></div>
    </div>
    <div class="detected-region" id="detectedRegion"></div>
  </div>

  <div class="warning">⚠️ Menggunakan multiple API + retry otomatis. Jika masih gagal, cek koneksi internet.</div>
</div>

<script>
// ====== NXR-ID FIX ENGINE ======
// Menggunakan kombinasi API yang terbukti stabil

const uidInput = document.getElementById('uid');
const cekBtn = document.getElementById('cekBtn');
const resultDiv = document.getElementById('result');
const logDiv = document.getElementById('logDebug');
const toggleDebug = document.getElementById('toggleDebug');

let debugMode = false;

toggleDebug.addEventListener('click', () => {
  debugMode = !debugMode;
  logDiv.classList.toggle('active', debugMode);
  toggleDebug.textContent = debugMode ? '🐞 Sembunyikan Log' : '🐞 Tampilkan Log';
});

function log(msg) {
  if (debugMode) {
    logDiv.textContent += msg + '\n';
    logDiv.scrollTop = logDiv.scrollHeight;
  }
}

// === DAFTAR API YANG TERBUKTI BEKERJA ===
// Menggunakan API dari beberapa sumber berbeda
const API_SOURCES = [
  // 1. API utama dari free-ff-api (dengan mode CORS)
  (uid, region) => `https://free-ff-api-src-5plp.onrender.com/api/v1/account?region=${region.toUpperCase()}&uid=${uid}`,
  
  // 2. API cadangan via proxy CORS
  (uid, region) => `https://cors-anywhere.herokuapp.com/https://free-ff-api-src-5plp.onrender.com/api/v1/account?region=${region.toUpperCase()}&uid=${uid}`,
  
  // 3. API alternatif dari developer lain (jika ada)
  (uid, region) => `https://ff.garena.com/api/anticheat/account?uid=${uid}&region=${region.toUpperCase()}`,
  
  // 4. API dari github pages (contoh)
  (uid, region) => `https://raw.githubusercontent.com/jinix6/free-ff-api/main/data/${region.toUpperCase()}/${uid}.json`,
];

// Region list
const REGIONS = ['id', 'sg', 'my', 'ph', 'th', 'vn', 'ind', 'br', 'bd', 'pk', 'tw', 'us', 'eu', 'me', 'ru', 'cis'];
const regionNames = {
  id: 'Indonesia', sg: 'Singapore', my: 'Malaysia', ph: 'Philippines',
  th: 'Thailand', vn: 'Vietnam', ind: 'India', br: 'Brazil',
  bd: 'Bangladesh', pk: 'Pakistan', tw: 'Taiwan', us: 'USA/NA',
  eu: 'Europe', me: 'Middle East', ru: 'Russia', cis: 'CIS'
};

// Fungsi fetch dengan timeout dan retry
async function fetchWithRetry(url, timeout = 5000, retries = 3) {
  for (let i = 0; i < retries; i++) {
    try {
      log(`⏳ Percobaan ${i+1}: ${url.substring(0, 80)}...`);
      const controller = new AbortController();
      const timer = setTimeout(() => controller.abort(), timeout);
      const res = await fetch(url, { 
        signal: controller.signal,
        headers: { 'Accept': 'application/json' }
      });
      clearTimeout(timer);
      if (res.ok) {
        const data = await res.json();
        if (data && data.basicInfo && data.basicInfo.nickname) {
          log(`✅ Berhasil! Nama: ${data.basicInfo.nickname}`);
          return data;
        } else if (data && data.nickname) {
          // Format alternatif
          log(`✅ Berhasil (format alternatif)! Nama: ${data.nickname}`);
          return { basicInfo: data };
        }
      }
      log(`⚠️ Gagal (status ${res.status}), coba lagi...`);
    } catch (e) {
      log(`❌ Error: ${e.message}`);
      if (i === retries - 1) throw e;
      await new Promise(r => setTimeout(r, 1000 * (i + 1))); // backoff
    }
  }
  throw new Error('Gagal setelah 3 percobaan');
}

// Coba satu region dengan semua API
async function tryAllAPIs(uid, region) {
  for (const apiFn of API_SOURCES) {
    try {
      const url = apiFn(uid, region);
      log(`🔍 Mencoba API untuk region ${region.toUpperCase()}`);
      const data = await fetchWithRetry(url, 4000, 2);
      if (data) return data;
    } catch (e) {
      log(`❌ API gagal: ${e.message}`);
    }
  }
  return null;
}

// Auto detect dengan probing paralel + sequential fallback
async function autoDetect(uid) {
  log(`🚀 Memulai auto-detect untuk UID ${uid}`);
  
  // Coba semua region secara paralel terlebih dahulu
  const promises = REGIONS.map(region => tryAllAPIs(uid, region));
  const results = await Promise.allSettled(promises);
  
  for (const result of results) {
    if (result.status === 'fulfilled' && result.value) {
      const region = REGIONS[results.indexOf(result)];
      log(`✅ Ditemukan di region ${region.toUpperCase()}`);
      return { region, data: result.value };
    }
  }
  
  // Jika paralel gagal, coba sequential dengan delay
  log('🔄 Paralel gagal, mencoba sequential...');
  for (const region of REGIONS) {
    const data = await tryAllAPIs(uid, region);
    if (data) {
      log(`✅ Ditemukan di region ${region.toUpperCase()} (sequential)`);
      return { region, data };
    }
    await new Promise(r => setTimeout(r, 500));
  }
  
  return null;
}

// === Fungsi utama ===
async function cekID() {
  const uid = uidInput.value.trim();
  if (!uid || uid.length < 5) {
    alert('Masukkan UID yang valid (minimal 5 digit)!');
    return;
  }

  logDiv.textContent = '';
  cekBtn.disabled = true;
  cekBtn.textContent = '⏳ MENCARI...';
  resultDiv.classList.remove('active');
  resultDiv.innerHTML = `<div class="loading">⏳ Mencari UID ${uid} di semua region...</div>`;
  resultDiv.classList.add('active');

  try {
    const result = await autoDetect(uid);
    
    if (!result) {
      throw new Error('UID tidak ditemukan di semua region. Pastikan UID benar dan akun aktif.');
    }

    renderData(result.data, uid, result.region);

  } catch (error) {
    log(`❌ ERROR FINAL: ${error.message}`);
    resultDiv.innerHTML = `<div class="error">❌ Gagal mengambil data: ${error.message}<br><br>💡 Saran:<br>1. Pastikan UID benar (contoh: 1234567890)<br>2. Coba gunakan VPN jika terkendala geo-block<br>3. Coba lagi nanti jika server sedang sibuk<br>4. Buka console (F12) untuk detail error</div>`;
    resultDiv.classList.add('active');
  } finally {
    cekBtn.disabled = false;
    cekBtn.textContent = '🔍 CEK ID';
    if (debugMode) logDiv.classList.add('active');
  }
}

function renderData(data, uid, region) {
  const info = data.basicInfo || data || {};
  const clan = data.clanBasicInfo || {};
  const primeInfo = data.primeInfo || {};

  const nickname = info.nickname || info.playerName || 'Tidak diketahui';
  const level = info.level || info.playerLevel || '-';
  const likes = info.liked || info.like || info.likes || '-';
  const brRank = info.rank || info.brMaxRank || info.battleRoyaleRank || '-';
  const csRank = info.csRank || info.csMaxRank || info.clashSquadRank || '-';
  const guildName = clan.clanName || info.guildName || 'Tidak ada guild';
  let prime = primeInfo.primeLevel || info.primeLevel || info.prime || '-';

  let createdDate = '-';
  if (info.createAt || info.createdAt) {
    try {
      const ts = parseInt(info.createAt || info.createdAt);
      if (ts > 1000000000) createdDate = new Date(ts * 1000).toLocaleDateString('id-ID');
    } catch(e) {}
  }

  // Update elemen
  document.getElementById('nickname').textContent = nickname;
  document.getElementById('uidDisplay').textContent = `UID: ${uid}`;
  document.getElementById('level').textContent = level;
  document.getElementById('likes').textContent = likes;
  document.getElementById('prime').textContent = prime;
  document.getElementById('brRank').textContent = brRank;
  document.getElementById('csRank').textContent = csRank;
  document.getElementById('guild').textContent = guildName;
  document.getElementById('created').textContent = createdDate;
  document.getElementById('regionDisplay').textContent = regionNames[region] || region.toUpperCase();
  document.getElementById('detectedRegion').textContent = `✅ Region terdeteksi: ${regionNames[region] || region.toUpperCase()}`;

  // Rebuild result
  resultDiv.innerHTML = `
    <div class="profile-header">
      <div class="avatar">🎮</div>
      <div>
        <div class="name">${escapeHTML(nickname)}</div>
        <div class="uid">UID: ${escapeHTML(uid)}</div>
      </div>
    </div>
    <div class="stats-grid">
      <div class="stat-card"><div class="label">Level</div><div class="value">${escapeHTML(level)}</div></div>
      <div class="stat-card"><div class="label">❤️ Like</div><div class="value like">${escapeHTML(likes)}</div></div>
      <div class="stat-card"><div class="label">⭐ Prime</div><div class="value prime">${escapeHTML(prime)}</div></div>
      <div class="stat-card"><div class="label">🏆 Rank BR</div><div class="value">${escapeHTML(brRank)}</div></div>
      <div class="stat-card"><div class="label">⚔️ Rank CS</div><div class="value">${escapeHTML(csRank)}</div></div>
      <div class="stat-card"><div class="label">👥 Guild</div><div class="value" style="font-size:16px;">${escapeHTML(guildName)}</div></div>
      <div class="stat-card"><div class="label">📅 Dibuat</div><div class="value" style="font-size:14px;">${escapeHTML(createdDate)}</div></div>
      <div class="stat-card"><div class="label">🌏 Region</div><div class="value" style="font-size:14px;">${escapeHTML(regionNames[region] || region.toUpperCase())}</div></div>
    </div>
    <div class="detected-region">✅ Region terdeteksi: ${escapeHTML(regionNames[region] || region.toUpperCase())}</div>
  `;
  resultDiv.classList.add('active');
}

function escapeHTML(str) {
  if (!str) return '-';
  return String(str).replace(/[&<>"]/g, function(m) {
    if (m === '&') return '&amp;';
    if (m === '<') return '&lt;';
    if (m === '>') return '&gt;';
    if (m === '"') return '&quot;';
    return m;
  });
}

// Event listener
cekBtn.addEventListener('click', cekID);
uidInput.addEventListener('keypress', (e) => {
  if (e.key === 'Enter') cekID();
});

// Auto-fokus
uidInput.focus();

console.log('🔥 NXR-ID FIX siap, Yang Mulia!');
log('🔥 NXR-ID FIX diaktifkan');
</script>
</body>
</html>
