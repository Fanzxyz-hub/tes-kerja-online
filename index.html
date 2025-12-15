<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tes Kerja Online – FINAL BOSS</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">
<style>
*{font-family:Poppins;box-sizing:border-box}
body{margin:0;min-height:100vh;background:linear-gradient(135deg,#4f46e5,#06b6d4);display:flex;justify-content:center;align-items:center}
.card{background:#fff;width:90%;max-width:480px;padding:24px;border-radius:18px;box-shadow:0 20px 40px rgba(0,0,0,.25)}
h2{text-align:center}
input{width:100%;padding:12px;border-radius:12px;border:1px solid #ddd;margin:8px 0}
button{width:100%;padding:12px;border:none;border-radius:14px;background:#4f46e5;color:#fff;font-size:16px;cursor:pointer}
.option{padding:12px;border-radius:14px;background:#f3f4f6;margin:8px 0;cursor:pointer;transition:.3s}
.option:hover{background:#e0e7ff}
.correct{background:#22c55e!important;color:#fff}
.wrong{background:#ef4444!important;color:#fff}
.disabled{pointer-events:none;opacity:.7}
.hidden{display:none}
.timer{text-align:center;font-weight:600;color:#ef4444}
</style>
</head>

<body>

<div class="card" id="login">
<h2>🚀 Tes Kerja Online</h2>
<input id="nama" placeholder="Nama">
<input id="posisi" placeholder="Posisi / Jabatan">
<button onclick="start()">Mulai Tes</button>
</div>

<div class="card hidden" id="quiz">
<div class="timer" id="timer">⏱️ 15</div>
<h2 id="nomor"></h2>
<p id="pertanyaan"></p>
<div id="opsi"></div>
<button onclick="next()">Next</button>
</div>

<div class="card hidden" id="hasilPage">
<h2>🎉 Hasil Akhir</h2>
<p id="hasil"></p>
<button onclick="kirimSemua()">Kirim Hasil</button>
</div>

<script>
/* ====== KONFIG GOOGLE FORM ====== */
const GOOGLE_FORM_URL =
"https://docs.google.com/forms/d/e/1FAIpQLSeFpMMISF0pOkiklwAibhDyFvLk68zMX_xJbCPcL4J3YhDPOg/formResponse";

const ENTRY_NAMA   = "entry.2118270270";
const ENTRY_POSISI = "entry.522712635";
const ENTRY_NILAI  = "entry.712560956";
/* ================================= */

const soal = [
{q:"Mobil : Bensin = Manusia :",o:["Makan","Tidur","Topi","Kursi"],a:0},
{q:"Mata : Melihat = Telinga :",o:["Berjalan","Mendengar","Minum","Tidur"],a:1},
{q:"Ikan : Air = Burung :",o:["Darat","Lumpur","Udara","Batu"],a:2},
{q:"Pena digunakan untuk",o:["Menulis","Memotong","Makan","Menjahit"],a:0},
{q:"Guru bekerja di",o:["Pasar","Sekolah","Bandara","Pabrik"],a:1},
{q:"Jam berfungsi untuk",o:["Menghitung uang","Menunjuk waktu","Memasak","Menimbang"],a:1},
{q:"Kunci : Pintu = Password :",o:["Internet","Akun","Monitor","Mouse"],a:1},
{q:"Api menghasilkan",o:["Air","Es","Panas","Angin"],a:2},
{q:"Laptop termasuk",o:["Alat musik","Perabot","Perangkat elektronik","Mainan"],a:2},
{q:"Indonesia berada di benua",o:["Eropa","Amerika","Asia","Afrika"],a:2},
{q:"Air mendidih pada suhu",o:["50°C","100°C","0°C","150°C"],a:1},
{q:"Alat untuk mengukur listrik",o:["Penggaris","Multimeter","Timbangan","Kompas"],a:1},
{q:"Bekerja tepat waktu disebut",o:["Malas","Disiplin","Ceroboh","Santai"],a:1},
{q:"Orang yang memimpin disebut",o:["Anggota","Ketua","Peserta","Penonton"],a:1},
{q:"Kerja sama dalam tim disebut",o:["Individu","Kompetisi","Teamwork","Konflik"],a:2}
];

let index=0,score=0,time=15,interval,answered=false;

window.onbeforeunload=()=> "Tes belum selesai";

function start(){
 if(!nama.value||!posisi.value){alert("Isi nama & posisi!");return;}
 localStorage.nama=nama.value;
 localStorage.posisi=posisi.value;
 index=0;score=0;
 login.classList.add("hidden");
 quiz.classList.remove("hidden");
 load();startTimer();
}

function load(){
 answered=false;time=15;
 let s=soal[index];
 nomor.innerText=`Soal ${index+1} / ${soal.length}`;
 pertanyaan.innerText=s.q;
 opsi.innerHTML="";
 s.o.forEach((op,i)=>{
  let d=document.createElement("div");
  d.className="option";
  d.innerText=op;
  d.onclick=()=>jawab(d,i);
  opsi.appendChild(d);
 });
}

function startTimer(){
 clearInterval(interval);
 interval=setInterval(()=>{
  timer.innerText=`⏱️ ${time}`;
  time--; if(time<0) next();
 },1000);
}

function jawab(el,i){
 if(answered)return;
 answered=true; clearInterval(interval);
 document.querySelectorAll(".option").forEach(o=>o.classList.add("disabled"));
 if(i===soal[index].a){el.classList.add("correct");score++;}
 else{el.classList.add("wrong");opsi.children[soal[index].a].classList.add("correct");}
}

function next(){
 if(!answered && time>=0){alert("Jawab dulu");return;}
 index++;
 if(index>=soal.length){
  quiz.classList.add("hidden");
  hasilPage.classList.remove("hidden");
  hasil.innerHTML=
   `Nama: ${localStorage.nama}<br>
    Posisi: ${localStorage.posisi}<br>
    Nilai: ${Math.round(score/soal.length*100)}%`;
  window.onbeforeunload=null;
 }else{load();startTimer();}
}

function kirimSemua(){
 const nilai=Math.round(score/soal.length*100);
 const fd=new FormData();
 fd.append(ENTRY_NAMA,localStorage.nama);
 fd.append(ENTRY_POSISI,localStorage.posisi);
 fd.append(ENTRY_NILAI,nilai);

 fetch(GOOGLE_FORM_URL,{method:"POST",mode:"no-cors",body:fd});
 alert("Hasil berhasil dikirim 🚀");
}
</script>
</body>
</html>