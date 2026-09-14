<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Sistema de Visitas - Demonstração</title>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:"Segoe UI",Arial,sans-serif}
body{background:#f4f5f7;color:#1f2937}
nav{background:#1f2937;padding:16px 24px;display:flex;gap:24px;flex-wrap:wrap}
nav a{color:#f9fafb;text-decoration:none;font-weight:600;cursor:pointer}
nav a:hover{color:#38bdf8}
.container{max-width:960px;margin:32px auto;padding:0 16px}
h1{margin-bottom:24px}
.section{display:none}
.active{display:block}
.banner-alerta{background:#fee2e2;color:#991b1b;padding:14px 18px;border-radius:8px;margin-bottom:16px;font-weight:600}
.sem-alertas{background:#dcfce7;color:#166534;padding:14px 18px;border-radius:8px}
.item-alerta{background:#fff;border-left:4px solid #ef4444;padding:12px 16px;border-radius:6px;margin-bottom:10px;box-shadow:0 1px 3px rgba(0,0,0,.08)}
.form-box{background:#fff;padding:20px;border-radius:8px;box-shadow:0 1px 3px rgba(0,0,0,.08);margin-bottom:24px}
input,select,textarea{width:100%;padding:10px;margin-bottom:12px;border:1px solid #d1d5db;border-radius:6px;font-size:14px}
button{background:#2563eb;color:#fff;border:none;padding:10px 18px;border-radius:6px;cursor:pointer;font-weight:600}
button:hover{background:#1d4ed8}
.card-cliente,.devolutiva-item,.historico-item{background:#fff;padding:16px;border-radius:8px;margin-bottom:12px;box-shadow:0 1px 3px rgba(0,0,0,.08)}
.info{font-size:13px;color:#6b7280;margin-bottom:8px}
.produto-linha{display:flex;align-items:center;gap:10px;font-size:13px;margin-bottom:6px;padding:6px;background:#f9fafb;border-radius:6px}
.cor-bolinha{width:18px;height:18px;border-radius:50%;border:1px solid #ccc;display:inline-block}
.acoes button{font-size:13px;padding:6px 12px;margin-right:8px;margin-top:6px}
.checkbox-cliente{display:flex;align-items:center;gap:10px;background:#fff;padding:10px 14px;border-radius:6px;margin-bottom:8px}
.checkbox-cliente input{width:auto}
.modal-bg{position:fixed;inset:0;background:rgba(0,0,0,.5);display:flex;align-items:center;justify-content:center;padding:16px;z-index:999}
.modal-box{background:#fff;padding:20px;border-radius:8px;width:100%;max-width:420px;max-height:90vh;overflow-y:auto}
.foto-preview{width:100%;max-height:150px;object-fit:cover;border-radius:6px;margin-bottom:12px}
.btn-cor-confirmar{background:#6b7280}
.btn-cor-confirmar.confirmado{background:#16a34a}
.tag-obrigatorio{color:#ef4444;font-size:12px}
</style>
</head>
<body>

<nav>
  <a onclick="mostrar('dashboard')">Dashboard</a>
  <a onclick="mostrar('clientes')">Clientes</a>
  <a onclick="mostrar('rota')">Montar Rota</a>
  <a onclick="mostrar('devolutiva')">Devolutiva</a>
  <a onclick="mostrar('historico')">Histórico</a>
</nav>

<div class="container">

  <section id="dashboard" class="section active">
    <h1>Painel de Visitas</h1>
    <div id="alertas-container"></div>
  </section>

  <section id="clientes" class="section">
    <h1>Clientes & Produtos</h1>
    <div class="form-box">
      <h3>Cadastrar novo cliente</h3>
      <input type="text" id="c-nome" placeholder="Nome do cliente">
      <input type="text" id="c-responsavel" placeholder="Responsável (vendedor)">
      <button onclick="cadastrarCliente()">Cadastrar</button>
    </div>
    <div id="lista-clientes"></div>
  </section>

  <section id="rota" class="section">
    <h1>Montar Rota</h1>
    <div class="form-box">
      <input type="text" id="r-responsavel" placeholder="Nome do vendedor responsável">
    </div>
    <div id="lista-clientes-rota"></div>
    <button onclick="criarRota()">Criar Rota + Gerar PDF</button>
  </section>

  <section id="devolutiva" class="section">
    <h1>Devolutiva da Rota</h1>
    <div class="form-box">
      <label>Selecione a rota pendente:</label>
      <select id="select-rota" onchange="abrirRota(this.value)"></select>
    </div>
    <div id="clientes-devolutiva"></div>
    <button id="btn-finalizar" style="display:none" onclick="finalizarRota()">Finalizar Rota</button>
  </section>

  <section id="historico" class="section">
    <h1>Histórico Geral</h1>
    <div id="lista-historico"></div>
  </section>

</div>

<script>
/* ---------------- UTILIDADES DE ARMAZENAMENTO ---------------- */
function getClientes(){ return JSON.parse(localStorage.getItem('clientes')||'[]'); }
function saveClientes(l){ localStorage.setItem('clientes', JSON.stringify(l)); }
function getRotas(){ return JSON.parse(localStorage.getItem('rotas')||'[]'); }
function saveRotas(l){ localStorage.setItem('rotas', JSON.stringify(l)); }
function getHistorico(){ return JSON.parse(localStorage.getItem('historico')||'[]'); }
function pushHistorico(descricao){
  const h = getHistorico();
  h.unshift({ data: new Date().toISOString(), descricao });
  localStorage.setItem('historico', JSON.stringify(h));
}
function novoId(){ return Date.now().toString(36) + Math.random().toString(36).slice(2,7); }
function formatarData(iso){ return iso ? new Date(iso).toLocaleString('pt-BR') : '—'; }

/* ---------------- NAVEGAÇÃO ---------------- */
function mostrar(id){
  document.querySelectorAll('.section').forEach(s=>s.classList.remove('active'));
  document.getElementById(id).classList.add('active');
  if(id==='dashboard') renderAlertas();
  if(id==='clientes') renderClientes();
  if(id==='rota') renderClientesRota();
  if(id==='devolutiva') renderRotasPendentes();
  if(id==='historico') renderHistorico();
}

/* ---------------- DASHBOARD ---------------- */
const DIAS_LIMITE = 30;
function renderAlertas(){
  const clientes = getClientes();
  const hoje = new Date();
  const atrasados = [];
  clientes.forEach(c=>{
    if(!c.ultimaVisita){ atrasados.push({...c, dias:null}); return; }
    const diff = Math.floor((hoje - new Date(c.ultimaVisita))/86400000);
    if(diff > DIAS_LIMITE) atrasados.push({...c, dias:diff});
  });
  atrasados.sort((a,b)=>(b.dias??9999)-(a.dias??9999));
  const container = document.getElementById('alertas-container');
  container.innerHTML = '';
  if(!atrasados.length){
    container.innerHTML = '<p class="sem-alertas">Nenhum cliente atrasado. Base em dia!</p>';
    return;
  }
  container.innerHTML = `<div class="banner-alerta">⚠️ ${atrasados.length} cliente(s) sem visita há mais de 30 dias</div>`;
  atrasados.forEach(c=>{
    container.innerHTML += `
      <div class="item-alerta">
        <strong>${c.nome}</strong><br>
        ${c.dias===null?'Nunca visitado':c.dias+' dias sem visita'}<br>
        Responsável: ${c.responsavel||'Não atribuído'}
      </div>`;
  });
}

/* ---------------- CLIENTES ---------------- */
function cadastrarCliente(){
  const nome = document.getElementById('c-nome').value.trim();
  const responsavel = document.getElementById('c-responsavel').value.trim();
  if(!nome){ alert('Informe o nome do cliente.'); return; }
  const clientes = getClientes();
  clientes.push({ id: novoId(), nome, responsavel, ultimaVisita:null, produtos:[] });
  saveClientes(clientes);
  pushHistorico(`Cliente cadastrado: ${nome}`);
  document.getElementById('c-nome').value='';
  document.getElementById('c-responsavel').value='';
  renderClientes();
}

function renderClientes(){
  const container = document.getElementById('lista-clientes');
  const clientes = getClientes();
  container.innerHTML = clientes.length ? '' : '<p>Nenhum cliente cadastrado.</p>';
  clientes.forEach(c=>{
    const produtosHtml = (c.produtos||[]).map(p=>`
      <div class="produto-linha">
        <span class="cor-bolinha" style="background:${p.cor}"></span>
        ${p.tipo}${p.nome ? ' - '+p.nome : ''} | Estoque: ${p.estoque||0} | Gôndola: ${p.gondola||0}
        ${p.foto ? '<img src="'+p.foto+'" style="width:30px;height:30px;border-radius:4px;object-fit:cover">' : ''}
      </div>`).join('');
    const div = document.createElement('div');
    div.className = 'card-cliente';
    div.innerHTML = `
      <h3>${c.nome}</h3>
      <div class="info">Responsável: ${c.responsavel||'—'} | Última visita: ${formatarData(c.ultimaVisita)}</div>
      ${produtosHtml}
      <div class="acoes">
        <button onclick="abrirModalProduto('${c.id}')">+ Produto</button>
        <button onclick="registrarVisita('${c.id}')">Registrar Visita Agora</button>
      </div>`;
    container.appendChild(div);
  });
}

function registrarVisita(id){
  const clientes = getClientes();
  const c = clientes.find(x=>x.id===id);
  c.ultimaVisita = new Date().toISOString();
  saveClientes(clientes);
  pushHistorico(`Visita registrada manualmente: ${c.nome}`);
  renderClientes();
  renderAlertas();
}

/* ---------------- MODAL DE PRODUTO ---------------- */
let corConfirmada = false;

function abrirModalProduto(clienteId){
  corConfirmada = false;
  const modal = document.createElement('div');
  modal.className = 'modal-bg';
  modal.innerHTML = `
    <div class="modal-box">
      <h3>Adicionar Produto</h3>

      <label>Tipo <span class="tag-obrigatorio">*obrigatório</span></label>
      <select id="p-tipo">
        <option value="">Selecione</option>
        <option>prata 925</option>
        <option>semijoia</option>
        <option>bijouteria</option>
        <option>óculos</option>
        <option>relógio</option>
        <option>aço inoxidável</option>
        <option>folheado</option>
        <option>bolsa</option>
      </select>

      <label>Nome do produto (opcional)</label>
      <input type="text" id="p-nome" placeholder="Ex: Anel solitário">

      <label>Cor <span class="tag-obrigatorio">*obrigatório</span></label>
      <input type="color" id="p-cor" value="#c0c0c0">
      <button type="button" class="btn-cor-confirmar" id="btn-confirmar-cor" onclick="confirmarCor()">Confirmar Cor</button>

      <label style="margin-top:12px;display:block;">Quantidade em Estoque (opcional)</label>
      <input type="number" id="p-estoque" placeholder="0">

      <label>Quantidade na Gôndola (opcional)</label>
      <input type="number" id="p-gondola" placeholder="0">

      <label>Foto (opcional)</label>
      <input type="file" id="p-foto" accept="image/*" capture="environment">
      <img id="p-foto-preview" class="foto-preview" style="display:none">

      <div style="margin-top:14px;">
        <button onclick="salvarProduto('${clienteId}')">Salvar Produto</button>
        <button style="background:#6b7280" onclick="this.closest('.modal-bg').remove()">Cancelar</button>
      </div>
    </div>`;
  document.body.appendChild(modal);

  document.getElementById('p-foto').addEventListener('change', function(e){
    const file = e.target.files[0];
    if(!file) return;
    const reader = new FileReader();
    reader.onload = function(ev){
      const preview = document.getElementById('p-foto-preview');
      preview.src = ev.target.result;
      preview.style.display = 'block';
    };
    reader.readAsDataURL(file);
  });
}

function confirmarCor(){
  corConfirmada = true;
  const btn = document.getElementById('btn-confirmar-cor');
  btn.textContent = 'Cor confirmada ✓';
  btn.classList.add('confirmado');
  document.getElementById('p-cor').disabled = true;
}

function salvarProduto(clienteId){
  const tipo = document.getElementById('p-tipo').value;
  const nome = document.getElementById('p-nome').value.trim();
  const cor = document.getElementById('p-cor').value;
  const estoque = Number(document.getElementById('p-estoque').value) || 0;
  const gondola = Number(document.getElementById('p-gondola').value) || 0;
  const fotoPreview = document.getElementById('p-foto-preview');
  const foto = fotoPreview.style.display !== 'none' ? fotoPreview.src : '';

  if(!tipo){ alert('Selecione o tipo do produto.'); return; }
  if(!corConfirmada){ alert('Confirme a cor antes de salvar.'); return; }

  const clientes = getClientes();
  const cliente = clientes.find(c=>c.id===clienteId);
  cliente.produtos = cliente.produtos || [];
  cliente.produtos.push({ id: novoId(), tipo, nome, cor, estoque, gondola, foto });
  saveClientes(clientes);
  pushHistorico(`Produto adicionado para ${cliente.nome}: ${tipo}${nome?' - '+nome:''} (cor ${cor})`);

  document.querySelector('.modal-bg').remove();
  renderClientes();
}

/* ---------------- ROTA ---------------- */
function renderClientesRota(){
  const container = document.getElementById('lista-clientes-rota');
  const clientes = getClientes();
  container.innerHTML = clientes.length ? '' : '<p>Cadastre clientes primeiro.</p>';
  clientes.forEach(c=>{
    container.innerHTML += `
      <div class="checkbox-cliente">
        <input type="checkbox" id="chk-${c.id}" value="${c.id}">
        <label for="chk-${c.id}">${c.nome}</label>
      </div>`;
  });
}

function criarRota(){
  const responsavel = document.getElementById('r-responsavel').value.trim();
  if(!responsavel){ alert('Informe o vendedor responsável.'); return; }

  const clientes = getClientes();
  const selecionados = clientes.filter(c => document.getElementById(`chk-${c.id}`)?.checked);
  if(!selecionados.length){ alert('Selecione ao menos um cliente.'); return; }

  const rota = {
    id: novoId(),
    data: new Date().toISOString(),
    responsavel,
    status: 'planejada',
    clientes: selecionados.map(c=>({ clienteId:c.id, nome:c.nome, status:'pendente', devolutiva:'' }))
  };

  const rotas = getRotas();
  rotas.push(rota);
  saveRotas(rotas);
  pushHistorico(`Rota criada por ${responsavel} com ${selecionados.length} cliente(s)`);

  gerarPdfRota(rota);
  alert('Rota criada e PDF gerado com sucesso!');
}

function gerarPdfRota(rota){
  const { jsPDF } = window.jspdf;
  const pdf = new jsPDF();
  const data = new Date(rota.data).toLocaleDateString('pt-BR');

  pdf.setFontSize(16);
  pdf.text('Relatório de Rota de Visitas', 14, 20);
  pdf.setFontSize(11);
  pdf.text(`Responsável: ${rota.responsavel}`, 14, 30);
  pdf.text(`Data: ${data}`, 14, 37);

  let y = 50;
  pdf.setFontSize(12);
  pdf.text('Clientes a visitar:', 14, y);
  y += 8;
  rota.clientes.forEach((c,i)=>{
    pdf.setFontSize(10);
    pdf.text(`${i+1}. ${c.nome}`, 18, y);
    y += 7;
  });

  pdf.save(`rota_${rota.responsavel}_${data}.pdf`);
}

/* ---------------- DEVOLUTIVA ---------------- */
function renderRotasPendentes(){
  const sel = document.getElementById('select-rota');
  const rotas = getRotas().filter(r=>r.status==='planejada');
  sel.innerHTML = '<option value="">Selecione</option>';
  rotas.forEach(r=>{
    sel.innerHTML += `<option value="${r.id}">${r.responsavel} - ${new Date(r.data).toLocaleDateString('pt-BR')}</option>`;
  });
  document.getElementById('clientes-devolutiva').innerHTML = '';
  document.getElementById('btn-finalizar').style.display = 'none';
}

function abrirRota(rotaId){
  const container = document.getElementById('clientes-devolutiva');
  container.innerHTML = '';
  if(!rotaId){ document.getElementById('btn-finalizar').style.display='none'; return; }

  const rota = getRotas().find(r=>r.id===rotaId);
  rota.clientes.forEach((c,i)=>{
    container.innerHTML += `
      <div class="devolutiva-item">
        <strong>${c.nome}</strong>
        <textarea id="dev-${i}" rows="3" placeholder="Descreva o que aconteceu na visita..."></textarea>
      </div>`;
  });
  document.getElementById('btn-finalizar').style.display = 'inline-block';
  document.getElementById('btn-finalizar').dataset.rotaId = rotaId;
}

function finalizarRota(){
  const rotaId = document.getElementById('btn-finalizar').dataset.rotaId;
  const rotas = getRotas();
  const rota = rotas.find(r=>r.id===rotaId);

  rota.clientes.forEach((c,i)=>{
    c.status = 'realizada';
    c.devolutiva = document.getElementById(`dev-${i}`).value.trim() || 'Sem observação';
  });
  rota.status = 'concluida';
  saveRotas(rotas);

  const clientes = getClientes();
  rota.clientes.forEach(rc=>{
    const cliente = clientes.find(c=>c.id===rc.clienteId);
    if(cliente){
      cliente.ultimaVisita = new Date().toISOString();
      pushHistorico(`Visita concluída: ${cliente.nome} - Devolutiva: ${rc.devolutiva}`);
    }
  });
  saveClientes(clientes);

  alert('Rota finalizada com sucesso!');
  renderRotasPendentes();
  renderAlertas();
}

/* ---------------- HISTÓRICO ---------------- */
function renderHistorico(){
  const container = document.getElementById('lista-historico');
  const historico = getHistorico();
  container.innerHTML = historico.length ? '' : '<p>Nenhum registro ainda.</p>';
  historico.forEach(h=>{
    container.innerHTML += `
      <div class="historico-item">
        <div class="info">${formatarData(h.data)}</div>
        <div>${h.descricao}</div>
      </div>`;
  });
}

/* ---------------- INICIALIZAÇÃO ---------------- */
renderAlertas();
</script>
</body>
</html>
