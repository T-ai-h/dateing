<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>💌 เธอรู้จักฉันดีแค่ไหน?</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Sarabun:wght@300;400;600&display=swap" rel="stylesheet">
<style>
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

body {
  min-height: 100vh;
  background: linear-gradient(160deg, #fce8f0 0%, #fdf0f7 50%, #f0e8fc 100%);
  font-family: 'Sarabun', sans-serif;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 24px 16px;
}

/* Floating ambient blobs */
.blob {
  position: fixed;
  border-radius: 50%;
  filter: blur(60px);
  pointer-events: none;
  opacity: 0.35;
  animation: drift 12s ease-in-out infinite alternate;
}
.blob-1 { width: 300px; height: 300px; background: #f9b8d0; top: -80px; left: -80px; animation-duration: 10s; }
.blob-2 { width: 220px; height: 220px; background: #d4b8f9; bottom: -60px; right: -60px; animation-duration: 14s; }
@keyframes drift { from { transform: translate(0,0); } to { transform: translate(30px, 20px); } }

/* Main container */
.app {
  width: 100%;
  max-width: 420px;
  position: relative;
  z-index: 1;
}

/* ── SCREENS ── */
.screen { display: none; flex-direction: column; align-items: center; gap: 0; }
.screen.active { display: flex; }

/* ── INTRO SCREEN ── */
.intro-card {
  background: rgba(255,255,255,0.82);
  backdrop-filter: blur(16px);
  border-radius: 32px;
  padding: 48px 36px 40px;
  text-align: center;
  box-shadow: 0 24px 64px rgba(200,80,140,0.13);
  border: 1px solid rgba(255,255,255,0.9);
  width: 100%;
}
.intro-emoji { font-size: 4rem; animation: bounce 2s ease-in-out infinite; display: block; margin-bottom: 20px; }
@keyframes bounce { 0%,100% { transform: translateY(0); } 50% { transform: translateY(-12px); } }
.intro-title {
  font-family: 'Playfair Display', serif;
  font-size: 1.75rem;
  font-weight: 700;
  color: #b03070;
  line-height: 1.3;
  margin-bottom: 10px;
}
.intro-sub {
  font-size: 0.95rem;
  color: #c080a0;
  line-height: 1.7;
  margin-bottom: 28px;
}
.intro-from {
  font-size: 0.78rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: #d4a0b8;
  margin-bottom: 28px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
}
.intro-from::before, .intro-from::after { content: '✦'; font-size: 0.6rem; }

/* Progress */
.progress-bar-wrap {
  background: #f4d8e8;
  border-radius: 99px;
  height: 6px;
  width: 100%;
  margin-bottom: 6px;
  overflow: hidden;
}
.progress-bar-fill {
  height: 100%;
  background: linear-gradient(90deg, #e878a8, #b03070);
  border-radius: 99px;
  transition: width 0.5s cubic-bezier(.4,0,.2,1);
}
.progress-text {
  font-size: 0.72rem;
  color: #c080a0;
  text-align: right;
  margin-bottom: 24px;
}

/* ── QUIZ SCREEN ── */
.quiz-card {
  background: rgba(255,255,255,0.85);
  backdrop-filter: blur(16px);
  border-radius: 28px;
  padding: 36px 28px 32px;
  box-shadow: 0 20px 56px rgba(200,80,140,0.12);
  border: 1px solid rgba(255,255,255,0.9);
  width: 100%;
}
.q-number {
  font-size: 0.72rem;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: #d4a0b8;
  margin-bottom: 10px;
}
.q-text {
  font-family: 'Playfair Display', serif;
  font-size: 1.22rem;
  color: #7a2850;
  line-height: 1.55;
  margin-bottom: 28px;
  min-height: 56px;
}
.choices { display: flex; flex-direction: column; gap: 10px; }
.choice-btn {
  background: #fff0f5;
  border: 1.5px solid #f0c8dc;
  border-radius: 14px;
  padding: 14px 18px;
  font-family: 'Sarabun', sans-serif;
  font-size: 0.95rem;
  color: #8a3860;
  text-align: left;
  cursor: pointer;
  transition: all 0.2s;
  display: flex;
  align-items: center;
  gap: 12px;
}
.choice-btn:hover:not(:disabled) {
  background: #fce0ec;
  border-color: #e878a8;
  transform: translateX(4px);
}
.choice-btn .choice-letter {
  width: 28px; height: 28px;
  border-radius: 50%;
  background: #f8d0e4;
  display: flex; align-items: center; justify-content: center;
  font-size: 0.72rem;
  font-weight: 600;
  color: #b03070;
  flex-shrink: 0;
  transition: all 0.2s;
}
.choice-btn.correct {
  background: #e8f8ef;
  border-color: #6cc990;
  color: #1a6640;
}
.choice-btn.correct .choice-letter { background: #6cc990; color: #fff; }
.choice-btn.wrong {
  background: #fde8ec;
  border-color: #e87890;
  color: #8a3848;
}
.choice-btn.wrong .choice-letter { background: #e87890; color: #fff; }
.choice-btn:disabled { cursor: default; transform: none; }

/* Feedback bubble */
.feedback {
  margin-top: 16px;
  padding: 12px 16px;
  border-radius: 12px;
  font-size: 0.9rem;
  line-height: 1.5;
  display: none;
  animation: pop 0.3s cubic-bezier(.34,1.56,.64,1);
}
@keyframes pop { from { transform: scale(0.85); opacity: 0; } to { transform: scale(1); opacity: 1; } }
.feedback.correct-fb { background: #e8f8ef; color: #1a6640; display: block; }
.feedback.wrong-fb   { background: #fde8ec; color: #8a3848; display: block; }

/* ── RESULT SCREEN ── */
.result-card {
  background: rgba(255,255,255,0.88);
  backdrop-filter: blur(16px);
  border-radius: 32px;
  padding: 44px 32px 40px;
  text-align: center;
  box-shadow: 0 24px 64px rgba(200,80,140,0.15);
  border: 1px solid rgba(255,255,255,0.9);
  width: 100%;
}
.result-emoji { font-size: 4.5rem; margin-bottom: 8px; display: block; animation: bounce 2s ease-in-out infinite; }
.result-score {
  font-family: 'Playfair Display', serif;
  font-size: 3.5rem;
  font-weight: 700;
  color: #b03070;
  line-height: 1;
  margin-bottom: 4px;
}
.result-score-label { font-size: 0.85rem; color: #d4a0b8; margin-bottom: 16px; }
.result-title {
  font-family: 'Playfair Display', serif;
  font-style: italic;
  font-size: 1.35rem;
  color: #7a2850;
  margin-bottom: 10px;
}
.result-msg {
  font-size: 0.95rem;
  color: #a05878;
  line-height: 1.7;
  margin-bottom: 28px;
  padding: 0 8px;
}
.hearts-row { display: flex; justify-content: center; gap: 6px; margin-bottom: 24px; }
.hearts-row span { font-size: 1.2rem; }

/* Shared button */
.btn-primary {
  background: linear-gradient(135deg, #e878a8, #b03070);
  color: #fff;
  border: none;
  border-radius: 14px;
  padding: 15px 36px;
  font-family: 'Sarabun', sans-serif;
  font-size: 1rem;
  font-weight: 600;
  cursor: pointer;
  box-shadow: 0 8px 24px rgba(176,48,112,0.28);
  transition: transform 0.18s, box-shadow 0.18s;
  width: 100%;
}
.btn-primary:hover { transform: translateY(-2px); box-shadow: 0 12px 32px rgba(176,48,112,0.36); }
.btn-secondary {
  background: #fff0f5;
  color: #b03070;
  border: 1.5px solid #f0c8dc;
  border-radius: 14px;
  padding: 13px 36px;
  font-family: 'Sarabun', sans-serif;
  font-size: 0.95rem;
  cursor: pointer;
  transition: all 0.18s;
  width: 100%;
  margin-top: 10px;
}
.btn-secondary:hover { background: #fce8f0; }

/* Next btn row */
.next-row { margin-top: 20px; display: none; }
.next-row.show { display: block; }

/* Confetti */
.confetti-piece {
  position: fixed;
  width: 8px; height: 8px;
  border-radius: 2px;
  pointer-events: none;
  animation: confetti-fall linear forwards;
  z-index: 999;
}
@keyframes confetti-fall {
  0%   { transform: translateY(-20px) rotate(0deg); opacity: 1; }
  100% { transform: translateY(100vh) rotate(720deg); opacity: 0; }
}
</style>
</head>
<body>

<div class="blob blob-1"></div>
<div class="blob blob-2"></div>

<div class="app">

  <!-- INTRO -->
  <div class="screen active" id="screen-intro">
    <div class="intro-card">
      <span class="intro-emoji">💌</span>
      <h1 class="intro-title">เธอรู้จักฉัน<br>ดีแค่ไหน?</h1>
      <p class="intro-sub">ลองตอบคำถามเหล่านี้ดูสิ<br>แล้วจะรู้เองว่าเธอรู้จักฉันมากแค่ไหน 🥰</p>
      <div class="intro-from" id="intro-from-name">จากคนที่รักเธอ</div>
      <button class="btn-primary" onclick="startQuiz()">เริ่มเลย! 💕</button>
    </div>
  </div>

  <!-- QUIZ -->
  <div class="screen" id="screen-quiz">
    <div class="quiz-card">
      <div class="progress-bar-wrap">
        <div class="progress-bar-fill" id="progress-fill" style="width:0%"></div>
      </div>
      <div class="progress-text" id="progress-text">ข้อ 1 / 5</div>

      <div class="q-number" id="q-number">ข้อที่ 1</div>
      <div class="q-text" id="q-text">...</div>

      <div class="choices" id="choices-wrap"></div>
      <div class="feedback" id="feedback"></div>

      <div class="next-row" id="next-row">
        <button class="btn-primary" id="next-btn" onclick="nextQuestion()">ข้อถัดไป →</button>
      </div>
    </div>
  </div>

  <!-- RESULT -->
  <div class="screen" id="screen-result">
    <div class="result-card">
      <span class="result-emoji" id="result-emoji">🎉</span>
      <div class="result-score" id="result-score">0/5</div>
      <div class="result-score-label">คะแนน</div>
      <div class="result-title" id="result-title">...</div>
      <div class="hearts-row" id="result-hearts"></div>
      <p class="result-msg" id="result-msg">...</p>
      <button class="btn-primary" onclick="shareResult()">แชร์ผลลัพธ์ 💕</button>
      <button class="btn-secondary" onclick="resetQuiz()">เล่นอีกครั้ง 🔁</button>
    </div>
  </div>

</div>

<script>
// ─── คำถาม (แก้ไขได้เลย!) ───────────────────────────────────────────
const quizData = {
  from: "จากคนที่รักเธอสุดใจ 💗",
  questions: [
    {
      q: "สีที่ฉันชอบมากที่สุดคือสีอะไร?",
      choices: ["สีชมพู 🌸", "สีฟ้า 🩵", "สีม่วง 💜", "สีเขียว 🍃"],
      correct: 0,
      feedback_correct: "ใช่เลย! เธอรู้จักฉันดีมาก 💕",
      feedback_wrong: "ยังไม่ใช่นะ… ฉันชอบสีชมพูค่ะ 🌸"
    },
    {
      q: "ฉันชอบกินอาหารอะไรมากที่สุด?",
      choices: ["ข้าวมันไก่ 🍗", "ราเมง 🍜", "ส้มตำ 🌶️", "พิซซ่า 🍕"],
      correct: 0,
      feedback_correct: "โอ้โห จำได้ด้วย! ฉันรักข้าวมันไก่ 🍜",
      feedback_wrong: "เปล่าเลย~ ฉันชอบข้าวมันไก่มากกว่านะ 🍜"
    },
    {
      q: "ถ้าฉันเครียด ฉันชอบทำอะไร?",
      choices: ["ฟังเพลง 🎵", "ดูซีรีส์ 📺", "กินของอร่อย 🍰", "นอนหลับ 😴"],
      correct: 0,
      feedback_correct: "เธอรู้ดีเลย! เพลงคือยาของฉันเลย 🎵",
      feedback_wrong: "ไม่ใช่นะ~ ฉันชอบเปิดเพลงเวลาเครียดมากกว่า 🎵"
    },
    {
      q: "สัตว์ที่ฉันอยากเลี้ยงที่สุดคืออะไร?",
      choices: ["สุนัข 🐶", "แมว 🐱", "กระต่าย 🐰", "นกแก้ว 🦜"],
      correct: 0,
      feedback_correct: "ถูกต้อง! หมาน่ารักมากจริงๆ 🐰",
      feedback_wrong: "ยังไม่ใช่เลย~ ฉันอยากเลี้ยงหมามากเลย 🐰"
    },
    {
      q: "ฉันฝันอยากไปเที่ยวที่ไหนมากที่สุด?",
      choices: ["ญี่ปุ่น 🇯🇵", "ยุโรป 🏰", "มัลดีฟส์ 🌊", "เกาหลี 🇰🇷"],
      correct: 0,
      feedback_correct: "เธอรู้จักฉันดีมากเลย! ไปด้วยกันนะ 🇯🇵💕",
      feedback_wrong: "เปล่าเลย~ ฉันอยากไปญี่ปุ่นมากที่สุดเลย 🇯🇵"
    }
  ]
};

const results = [
  { min: 0, max: 1, emoji: "🥺", title: "เธอยังต้องเรียนรู้ฉันอีกนะ", msg: "ไม่เป็นไร~ เราจะมีเวลาอีกเยอะให้เธอได้รู้จักฉันมากขึ้น ฉันรักเธอเสมอ 💕", hearts: "🤍🤍🤍🤍🤍" },
  { min: 2, max: 2, emoji: "🙂", title: "เธอรู้จักฉันได้บ้างนะ", msg: "ยังมีอะไรอีกเยอะที่เธอยังไม่รู้เลย แต่เวลาที่เราอยู่ด้วยกัน ฉันมีความสุขเสมอ 💗", hearts: "💕🤍🤍🤍🤍" },
  { min: 3, max: 3, emoji: "😊", title: "เธอรู้จักฉันดีพอสมควรเลยนะ!", msg: "เธอใส่ใจฉันมากเลย ทำให้ฉันรู้สึกอบอุ่นมากๆ ฉันรักเธอนะ 💖", hearts: "💕💕💕🤍🤍" },
  { min: 4, max: 4, emoji: "🥰", title: "เธอรู้จักฉันดีมากเลย!", msg: "เธอช่างสังเกตและใส่ใจฉันมากจริงๆ ฉันดีใจมากที่มีเธออยู่ข้างๆ 💝", hearts: "💕💕💕💕🤍" },
  { min: 5, max: 5, emoji: "💖", title: "เธอรู้จักฉันดีที่สุดในโลก!", msg: "ฉันไม่เคยรู้สึกเลยว่าตัวเองถูกรักและเข้าใจขนาดนี้… ขอบคุณที่ใส่ใจฉันทุกรายละเอียด รักเธอมากที่สุด 💗", hearts: "💕💕💕💕💕" }
];

// ─── State ───────────────────────────────────────────────────────────
let current = 0;
let score = 0;
let answered = false;

function show(id) {
  document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
  document.getElementById(id).classList.add('active');
}

function startQuiz() {
  document.getElementById('intro-from-name').textContent = quizData.from;
  current = 0; score = 0;
  loadQuestion();
  show('screen-quiz');
}

function loadQuestion() {
  answered = false;
  const q = quizData.questions[current];
  const total = quizData.questions.length;
  const pct = (current / total) * 100;

  document.getElementById('progress-fill').style.width = pct + '%';
  document.getElementById('progress-text').textContent = `ข้อ ${current + 1} / ${total}`;
  document.getElementById('q-number').textContent = `ข้อที่ ${current + 1}`;
  document.getElementById('q-text').textContent = q.q;

  const letters = ['A','B','C','D'];
  const wrap = document.getElementById('choices-wrap');
  wrap.innerHTML = '';
  q.choices.forEach((c, i) => {
    const btn = document.createElement('button');
    btn.className = 'choice-btn';
    btn.innerHTML = `<span class="choice-letter">${letters[i]}</span>${c}`;
    btn.onclick = () => selectAnswer(i);
    wrap.appendChild(btn);
  });

  document.getElementById('feedback').className = 'feedback';
  document.getElementById('feedback').textContent = '';
  document.getElementById('next-row').classList.remove('show');

  const nextLabel = current < quizData.questions.length - 1 ? 'ข้อถัดไป →' : 'ดูผลลัพธ์ 💕';
  document.getElementById('next-btn').textContent = nextLabel;
}

function selectAnswer(idx) {
  if (answered) return;
  answered = true;

  const q = quizData.questions[current];
  const btns = document.querySelectorAll('.choice-btn');
  btns.forEach(b => b.disabled = true);

  const fb = document.getElementById('feedback');

  if (idx === q.correct) {
    score++;
    btns[idx].classList.add('correct');
    fb.className = 'feedback correct-fb';
    fb.textContent = '✅ ' + q.feedback_correct;
  } else {
    btns[idx].classList.add('wrong');
    btns[q.correct].classList.add('correct');
    fb.className = 'feedback wrong-fb';
    fb.textContent = '❌ ' + q.feedback_wrong;
  }

  document.getElementById('next-row').classList.add('show');
}

function nextQuestion() {
  current++;
  if (current < quizData.questions.length) {
    loadQuestion();
  } else {
    showResult();
  }
}

function showResult() {
  const total = quizData.questions.length;
  const r = results.find(r => score >= r.min && score <= r.max);

  document.getElementById('result-emoji').textContent = r.emoji;
  document.getElementById('result-score').textContent = `${score}/${total}`;
  document.getElementById('result-title').textContent = r.title;
  document.getElementById('result-msg').textContent = r.msg;
  document.getElementById('result-hearts').innerHTML = [...r.hearts].map(h => `<span>${h}</span>`).join('');

  show('screen-result');

  if (score >= 4) launchConfetti();
}

function resetQuiz() { startQuiz(); }

function shareResult() {
  const total = quizData.questions.length;
  const text = `ฉันได้ ${score}/${total} ในควิซ "เธอรู้จักฉันดีแค่ไหน?" 💌`;
  if (navigator.share) {
    navigator.share({ title: 'Love Quiz 💕', text });
  } else {
    navigator.clipboard.writeText(text).then(() => alert('คัดลอกแล้ว! ไปแปะในแชทได้เลย 💕'));
  }
}

function launchConfetti() {
  const colors = ['#f87cb4','#e878a8','#b03070','#f0d0e8','#d4a0c8','#ffffff'];
  for (let i = 0; i < 80; i++) {
    setTimeout(() => {
      const c = document.createElement('div');
      c.className = 'confetti-piece';
      c.style.left = Math.random() * 100 + 'vw';
      c.style.background = colors[Math.floor(Math.random() * colors.length)];
      c.style.width = (6 + Math.random() * 8) + 'px';
      c.style.height = (6 + Math.random() * 8) + 'px';
      c.style.animationDuration = (2 + Math.random() * 2) + 's';
      c.style.animationDelay = (Math.random() * 0.5) + 's';
      document.body.appendChild(c);
      setTimeout(() => c.remove(), 4000);
    }, i * 30);
  }
}

// Init
document.getElementById('intro-from-name').textContent = quizData.from;
</script>
</body>
</html>