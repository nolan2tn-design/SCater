let dailyTasks = [
  { time: "06:20-07:20", task: "晨讀英文 / 國文 + Podcast", done: false },
  { time: "自主學習50分", task: "數學或自然複習", done: false },
  { time: "19:30-21:20", task: "數學/自然 + 英文 + 國文/錯題", done: false },
  { time: "21:20-22:40", task: "單字複習 + 勵志Podcast", done: false }
];

let holidayTasks = [
  { time: "9:10-11:15", task: "數學A大題 / 自然綜合複習", done: false },
  { time: "16:30-17:00", task: "英文單字 + 文法", done: false },
  { time: "19:30-21:20", task: "英文閱讀寫作 / 國文", done: false }
];

function renderTasks() {
  const dailyBody = document.getElementById('daily-tasks');
  dailyBody.innerHTML = dailyTasks.map((item, i) => `
    <tr>
      <td>${item.time}</td>
      <td>${item.task}</td>
      <td class="text-center"><input type="checkbox" ${item.done ? 'checked' : ''} onchange="toggleDaily(${i})"></td>
    </tr>
  `).join('');

  const holidayBody = document.getElementById('holiday-tasks');
  holidayBody.innerHTML = holidayTasks.map((item, i) => `
    <tr>
      <td>${item.time}</td>
      <td>${item.task}</td>
      <td class="text-center"><input type="checkbox" ${item.done ? 'checked' : ''} onchange="toggleHoliday(${i})"></td>
    </tr>
  `).join('');
}

function toggleDaily(i) { dailyTasks[i].done = !dailyTasks[i].done; }
function toggleHoliday(i) { holidayTasks[i].done = !holidayTasks[i].done; }

function saveDailyCheckin() {
  const percent = document.getElementById('today-percent').value;
  const note = document.getElementById('today-note').value.trim();
  const date = new Date().toLocaleDateString('zh-TW', { year: 'numeric', month: '2-digit', day: '2-digit' });

  let records = JSON.parse(localStorage.getItem('studyRecords') || '[]');
  records.unshift({ date, percent, note });
  localStorage.setItem('studyRecords', JSON.stringify(records));

  alert('✅ 今日打卡已儲存！');
  loadHistory();
}

function loadHistory() {
  const container = document.getElementById('history-list');
  const records = JSON.parse(localStorage.getItem('studyRecords') || '[]');
  
  if (records.length === 0) {
    container.innerHTML = '<p class="text-gray-400 text-center py-8">還沒有打卡紀錄</p>';
    return;
  }

  container.innerHTML = records.map(r => `
    <div class="bg-white p-5 rounded-2xl shadow">
      <div class="flex justify-between items-center">
        <span class="font-medium">${r.date}</span>
        <span class="text-green-600 font-bold text-xl">${r.percent}%</span>
      </div>
      ${r.note ? `<p class="mt-3 text-gray-600">${r.note}</p>` : ''}
    </div>
  `).join('');
}

function showTab(n) {
  document.querySelectorAll('.tab-content').forEach(el => el.classList.add('hidden'));
  document.getElementById('tab' + n).classList.remove('hidden');
  
  document.querySelectorAll('.tab-btn').forEach((el, i) => el.classList.toggle('active', i === n));
}

// 初始化
document.addEventListener('DOMContentLoaded', () => {
  renderTasks();
  loadHistory();
  
  document.getElementById('today-date').textContent = new Date().toLocaleDateString('zh-TW');
  
  const slider = document.getElementById('today-percent');
  const show = document.getElementById('percent-show');
  slider.addEventListener('input', () => show.textContent = slider.value + '%');
  
  showTab(0);
});