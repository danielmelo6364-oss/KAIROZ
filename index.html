<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gestão Comercial</title>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>

  <style>
    :root {
      --black: #080808;
      --black-2: #121212;
      --black-3: #1c1c1c;
      --black-4: #292929;
      --border: #383838;
      --red: #e50914;
      --red-dark: #640b10;
      --white: #ffffff;
      --gray: #a7a7a7;
      --green: #2dcc83;
      --yellow: #f4c542;
      --blue: #4098f0;
      --purple: #a978ff;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      color: var(--white);
      background: var(--black);
      font-family: Arial, Helvetica, sans-serif;
    }

    button,
    input,
    select,
    textarea {
      font: inherit;
    }

    button,
    a {
      cursor: pointer;
    }

    button {
      color: var(--white);
    }

    .layout {
      min-height: 100vh;
    }

    .sidebar {
      position: fixed;
      z-index: 10;
      top: 0;
      bottom: 0;
      left: 0;
      width: 240px;
      padding: 20px 12px;
      overflow-y: auto;
      background: #050505;
      border-right: 1px solid var(--border);
    }

    .logo {
      margin: 0 10px 25px;
      color: var(--red);
      font-size: 23px;
      font-weight: bold;
    }

    .logo small {
      display: block;
      margin-top: 4px;
      color: var(--gray);
      font-size: 10px;
      font-weight: normal;
      letter-spacing: 1px;
    }

    .nav-button {
      width: 100%;
      margin: 3px 0;
      padding: 12px;
      border: 0;
      border-radius: 6px;
      background: transparent;
      color: #bdbdbd;
      text-align: left;
    }

    .nav-button:hover,
    .nav-button.active {
      background: var(--red);
      color: white;
    }

    .main {
      width: calc(100% - 240px);
      min-height: 100vh;
      margin-left: 240px;
      padding: 26px;
    }

    .topbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 15px;
      margin-bottom: 24px;
    }

    h1,
    h2,
    h3,
    p {
      margin-top: 0;
    }

    h1 {
      margin-bottom: 5px;
      font-size: 27px;
    }

    h2 {
      margin-bottom: 16px;
      font-size: 20px;
    }

    h3 {
      margin-bottom: 12px;
      font-size: 16px;
    }

    .muted {
      color: var(--gray);
      font-size: 13px;
    }

    .page {
      display: none;
    }

    .page.active {
      display: block;
    }

    .panel,
    .card {
      padding: 17px;
      border: 1px solid var(--border);
      border-radius: 8px;
      background: var(--black-2);
    }

    .panel {
      margin-bottom: 15px;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 14px;
      margin-bottom: 15px;
    }

    .metric-label {
      color: var(--gray);
      font-size: 11px;
      letter-spacing: .5px;
      text-transform: uppercase;
    }

    .metric-value {
      margin-top: 9px;
      font-size: 25px;
      font-weight: bold;
    }

    .green {
      color: var(--green);
    }

    .red {
      color: var(--red);
    }

    .yellow {
      color: var(--yellow);
    }

    .blue {
      color: var(--blue);
    }

    .purple {
      color: var(--purple);
    }

    .grid-2,
    .grid-3,
    .grid-4 {
      display: grid;
      gap: 12px;
    }

    .grid-2 {
      grid-template-columns: repeat(2, 1fr);
    }

    .grid-3 {
      grid-template-columns: repeat(3, 1fr);
    }

    .grid-4 {
      grid-template-columns: repeat(4, 1fr);
    }

    .field {
      display: flex;
      flex-direction: column;
      gap: 6px;
    }

    .field.full {
      grid-column: 1 / -1;
    }

    label {
      color: #d4d4d4;
      font-size: 12px;
    }

    input,
    select,
    textarea {
      width: 100%;
      padding: 10px;
      outline: none;
      border: 1px solid var(--border);
      border-radius: 5px;
      background: #0b0b0b;
      color: white;
    }

    input:focus,
    select:focus,
    textarea:focus {
      border-color: var(--red);
    }

    input[readonly] {
      color: var(--green);
    }

    textarea {
      min-height: 80px;
      resize: vertical;
    }

    input[type="color"] {
      height: 40px;
      padding: 3px;
    }

    .actions {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-top: 14px;
    }

    .button {
      padding: 9px 13px;
      border: 1px solid var(--border);
      border-radius: 5px;
      background: var(--black-3);
      color: white;
    }

    .button:hover {
      filter: brightness(1.25);
    }

    .button.primary {
      border-color: var(--red);
      background: var(--red);
    }

    .button.success {
      border-color: #19724e;
      background: #095e3c;
    }

    .button.danger {
      border-color: #8f151c;
      background: #4d0c11;
    }

    .button.small {
      padding: 6px 9px;
      font-size: 12px;
    }

    .toolbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 12px;
      margin-bottom: 14px;
    }

    .toolbar input {
      max-width: 320px;
    }

    .table-container {
      overflow-x: auto;
    }

    table {
      width: 100%;
      min-width: 850px;
      border-collapse: collapse;
    }

    th,
    td {
      padding: 10px 8px;
      border-bottom: 1px solid var(--border);
      text-align: left;
      vertical-align: middle;
      font-size: 13px;
    }

    th {
      color: var(--gray);
      font-size: 11px;
      text-transform: uppercase;
    }

    tr.clickable {
      cursor: pointer;
    }

    tr.clickable:hover {
      background: #242424;
    }

    .badge {
      display: inline-flex;
      align-items: center;
      gap: 4px;
      padding: 4px 8px;
      border-radius: 20px;
      font-size: 11px;
      white-space: nowrap;
    }

    .badge-a {
      background: #691019;
      color: #ff9aa0;
    }

    .badge-b {
      background: #62500c;
      color: #ffdf65;
    }

    .badge-c {
      background: #104b76;
      color: #83c4ff;
    }

    .badge-active {
      background: #075b3b;
      color: #7df0bd;
    }

    .badge-inactive {
      background: #571018;
      color: #ff969c;
    }

    .badge-warning {
      background: #564207;
      color: #ffdd67;
    }

    .chips {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
    }

    .chip {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      padding: 5px 8px;
      border: 1px solid #444;
      border-radius: 20px;
      background: #282828;
      font-size: 11px;
      white-space: nowrap;
    }

    .chip.inactive {
      border-color: #2b2b2b;
      background: #171717;
      color: #777;
    }

    .dot {
      display: inline-block;
      width: 9px;
      height: 9px;
      border-radius: 50%;
    }

    .list {
      display: flex;
      flex-direction: column;
      gap: 8px;
    }

    .list-item {
      padding: 10px;
      border: 1px solid var(--border);
      border-radius: 6px;
      background: #101010;
    }

    .list-item strong {
      display: block;
      margin-bottom: 5px;
    }

    .empty {
      padding: 22px 10px;
      color: var(--gray);
      text-align: center;
      font-size: 13px;
    }

    .alert {
      margin-bottom: 14px;
      padding: 12px;
      border-left: 4px solid var(--yellow);
      border-radius: 5px;
      background: #261f08;
      color: #f4d97b;
      font-size: 13px;
    }

    .alert.red-alert {
      border-left-color: var(--red);
      background: #2a0a0d;
      color: #ffafb4;
    }

    .alert.green-alert {
      border-left-color: var(--green);
      background: #082b1d;
      color: #89e5b9;
    }

    .progress {
      height: 12px;
      overflow: hidden;
      border-radius: 20px;
      background: #292929;
    }

    .progress-bar {
      height: 100%;
      border-radius: 20px;
      background: linear-gradient(90deg, var(--red), #ff4851);
    }

    .sale-line {
      display: grid;
      grid-template-columns: 180px 1fr 90px 115px 38px;
      align-items: end;
      gap: 8px;
      margin-bottom: 9px;
    }

    .line-total {
      padding-bottom: 10px;
      color: var(--green);
      font-size: 13px;
      font-weight: bold;
    }

    .modal {
      position: fixed;
      z-index: 30;
      inset: 0;
      display: none;
      align-items: center;
      justify-content: center;
      padding: 20px;
      background: rgba(0, 0, 0, .8);
    }

    .modal.open {
      display: flex;
    }

    .modal-content {
      width: min(1050px, 100%);
      max-height: 92vh;
      overflow-y: auto;
      padding: 20px;
      border: 1px solid #444;
      border-top: 3px solid var(--red);
      border-radius: 8px;
      background: var(--black-2);
    }

    .modal-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 17px;
    }

    .close {
      border: 0;
      background: transparent;
      color: #aaa;
      font-size: 25px;
    }

    .profile-header {
      display: flex;
      align-items: flex-start;
      justify-content: space-between;
      gap: 15px;
      margin-bottom: 18px;
    }

    .profile-columns {
      display: grid;
      grid-template-columns: 1.1fr .9fr;
      gap: 15px;
    }

    .abc-row-a {
      border-left: 5px solid var(--red);
      background: rgba(229, 9, 20, .13);
    }

    .abc-row-b {
      border-left: 5px solid var(--yellow);
      background: rgba(244, 197, 66, .12);
    }

    .abc-row-c {
      border-left: 5px solid var(--blue);
      background: rgba(64, 152, 240, .12);
    }

    .abc-row-a:hover {
      background: rgba(229, 9, 20, .24) !important;
    }

    .abc-row-b:hover {
      background: rgba(244, 197, 66, .23) !important;
    }

    .abc-row-c:hover {
      background: rgba(64, 152, 240, .23) !important;
    }

    .abc-big {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      min-width: 62px;
      padding: 6px 8px;
      border-radius: 5px;
      font-weight: bold;
    }

    .abc-big.a {
      background: var(--red);
      color: white;
    }

    .abc-big.b {
      background: #d5af16;
      color: #111;
    }

    .abc-big.c {
      background: #1676c5;
      color: white;
    }

    @media (max-width: 1100px) {
      .cards {
        grid-template-columns: repeat(2, 1fr);
      }

      .profile-columns {
        grid-template-columns: 1fr;
      }
    }

    @media (max-width: 760px) {
      .sidebar {
        width: 65px;
        padding: 15px 7px;
      }

      .logo {
        margin: 0 0 25px;
        font-size: 0;
        text-align: center;
      }

      .logo::before {
        content: "G";
        font-size: 24px;
      }

      .logo small,
      .nav-button span {
        display: none;
      }

      .nav-button {
        padding: 12px 5px;
        text-align: center;
        font-size: 17px;
      }

      .main {
        width: calc(100% - 65px);
        margin-left: 65px;
        padding: 15px;
      }

      .grid-2,
      .grid-3,
      .grid-4 {
        grid-template-columns: 1fr;
      }

      .cards {
        grid-template-columns: 1fr 1fr;
        gap: 8px;
      }

      .metric-value {
        font-size: 20px;
      }

      .sale-line {
        grid-template-columns: 1fr 75px 100px 35px;
      }

      .sale-line .seller-field,
      .sale-line .product-field {
        grid-column: 1 / -1;
      }

      .profile-header {
        flex-direction: column;
      }
    }
  </style>
</head>

<body>
  <div class="layout">
    <aside class="sidebar">
      <div class="logo">
        GESTÃO
        <small>representação comercial</small>
      </div>

      <button class="nav-button active" data-page="dashboard">▣ <span>Dashboard</span></button>
      <button class="nav-button" data-page="clientes">♙ <span>Clientes</span></button>
      <button class="nav-button" data-page="produtos">▤ <span>Produtos</span></button>
      <button class="nav-button" data-page="fornecedores">◉ <span>Fornecedores</span></button>
      <button class="nav-button" data-page="vendedores">♟ <span>Vendedores</span></button>
      <button class="nav-button" data-page="financeiro">$ <span>Financeiro</span></button>
      <button class="nav-button" data-page="abc">▥ <span>Curva ABC</span></button>
    </aside>

    <main class="main">
      <div class="topbar">
        <div>
          <h1 id="page-title">Dashboard</h1>
          <div class="muted">Gestão comercial, metas e oportunidades</div>
        </div>

        <button class="button primary" onclick="openSaleModal()">
          + Nova venda
        </button>
      </div>

      <!-- DASHBOARD -->
      <section class="page active" id="page-dashboard">
        <div id="dashboard-alerts"></div>

        <div class="panel">
          <div class="toolbar">
            <div>
              <h2>Meta de vendas</h2>
              <div class="muted">
                A meta diária é calculada automaticamente pela meta mensal.
              </div>
            </div>

            <button class="button small" onclick="openSettingsModal()">
              Configurar meta
            </button>
          </div>

          <div class="cards">
            <div class="card">
              <div class="metric-label">Meta mensal</div>
              <div class="metric-value" id="goal-month">R$ 0,00</div>
            </div>

            <div class="card">
              <div class="metric-label">Meta diária calculada</div>
              <div class="metric-value yellow" id="goal-daily">R$ 0,00</div>
            </div>

            <div class="card">
              <div class="metric-label">Vendido no mês</div>
              <div class="metric-value green" id="goal-sold">R$ 0,00</div>
            </div>

            <div class="card">
              <div class="metric-label">Falta vender</div>
              <div class="metric-value red" id="goal-missing">R$ 0,00</div>
            </div>
          </div>

          <div class="progress">
            <div class="progress-bar" id="goal-progress"></div>
          </div>

          <div class="muted" id="goal-summary" style="margin-top:9px"></div>
        </div>

        <div class="cards">
          <div class="card">
            <div class="metric-label">Clientes</div>
            <div class="metric-value" id="metric-clients">0</div>
          </div>

          <div class="card">
            <div class="metric-label">Produtos</div>
            <div class="metric-value" id="metric-products">0</div>
          </div>

          <div class="card">
            <div class="metric-label">Vendas</div>
            <div class="metric-value" id="metric-sales">0</div>
          </div>

          <div class="card">
            <div class="metric-label">Faturamento geral</div>
            <div class="metric-value green" id="metric-revenue">R$ 0,00</div>
          </div>
        </div>

        <div class="grid-2">
          <div class="panel">
            <h2>Aniversariantes do mês</h2>
            <div id="birthdays-list"></div>
          </div>

          <div class="panel">
            <h2>Oportunidades de expansão</h2>
            <div id="expansion-list"></div>
          </div>
        </div>

        <div class="grid-2">
          <div class="panel">
            <h2>Clientes inativos</h2>
            <div id="inactive-list"></div>
          </div>

          <div class="panel">
            <h2>Produtos sem pedidos</h2>
            <div id="unused-products"></div>
          </div>
        </div>
      </section>

      <!-- CLIENTES -->
      <section class="page" id="page-clientes">
        <div class="panel">
          <h2>Cadastrar cliente</h2>

          <form id="client-form">
            <div class="grid-3">
              <div class="field">
                <label>Nome completo *</label>
                <input id="client-name" required>
              </div>

              <div class="field">
                <label>Telefone / WhatsApp</label>
                <input id="client-phone">
              </div>

              <div class="field">
                <label>E-mail</label>
                <input id="client-email" type="email">
              </div>

              <div class="field">
                <label>Data de nascimento</label>
                <input id="client-birth" type="date">
              </div>

              <div class="field">
                <label>Cidade</label>
                <input id="client-city">
              </div>

              <div class="field">
                <label>Observações</label>
                <input id="client-notes">
              </div>
            </div>

            <div class="actions">
              <button class="button primary">Salvar cliente</button>
            </div>
          </form>
        </div>

        <div class="panel">
          <div class="toolbar">
            <h2>Clientes cadastrados</h2>
            <input id="client-search" placeholder="Buscar cliente..." oninput="renderClients()">
          </div>

          <div class="table-container">
            <table>
              <thead>
                <tr>
                  <th>Cliente</th>
                  <th>Contato</th>
                  <th>Última compra</th>
                  <th>Status</th>
                  <th>Pedidos</th>
                  <th>Faturamento</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="clients-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- PRODUTOS -->
      <section class="page" id="page-produtos">
        <div class="panel">
          <h2>Cadastrar produto</h2>

          <form id="product-form">
            <div class="grid-3">
              <div class="field">
                <label>SKU *</label>
                <input id="product-sku" required>
              </div>

              <div class="field">
                <label>Nome do produto *</label>
                <input id="product-name" required>
              </div>

              <div class="field">
                <label>Fornecedor *</label>
                <select id="product-supplier" required></select>
              </div>

              <div class="field">
                <label>Preço de venda *</label>
                <input id="product-price" type="number" min="0" step="0.01" required>
              </div>

              <div class="field">
                <label>Categoria</label>
                <input id="product-category">
              </div>

              <div class="field">
                <label>Garantia em dias</label>
                <input id="product-warranty" type="number" min="0" value="0">
              </div>

              <div class="field full">
                <label>Observações</label>
                <textarea id="product-notes"></textarea>
              </div>
            </div>

            <div class="actions">
              <button class="button primary">Salvar produto</button>
            </div>
          </form>
        </div>

        <div class="panel">
          <div class="toolbar">
            <h2>Produtos cadastrados</h2>
            <input id="product-search" placeholder="Buscar produto ou SKU..." oninput="renderProducts()">
          </div>

          <div class="table-container">
            <table>
              <thead>
                <tr>
                  <th>SKU</th>
                  <th>Produto</th>
                  <th>Fornecedor</th>
                  <th>Categoria</th>
                  <th>Preço</th>
                  <th>Curva</th>
                  <th>Vendidos</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="products-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- FORNECEDORES -->
      <section class="page" id="page-fornecedores">
        <div class="panel">
          <h2>Cadastrar fornecedor</h2>

          <form id="supplier-form">
            <div class="grid-3">
              <div class="field">
                <label>Nome do fornecedor *</label>
                <input id="supplier-name" required>
              </div>

              <div class="field">
                <label>Contato</label>
                <input id="supplier-contact">
              </div>

              <div class="field">
                <label>Cor do fornecedor</label>
                <input id="supplier-color" type="color" value="#e50914">
              </div>
            </div>

            <div class="actions">
              <button class="button primary">Salvar fornecedor</button>
            </div>
          </form>
        </div>

        <div class="panel">
          <h2>Fornecedores cadastrados</h2>

          <div class="table-container">
            <table>
              <thead>
                <tr>
                  <th>Fornecedor</th>
                  <th>Contato</th>
                  <th>Produtos</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="suppliers-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- VENDEDORES -->
      <section class="page" id="page-vendedores">
        <div class="panel">
          <h2>Cadastrar vendedor</h2>

          <form id="seller-form">
            <div class="grid-3">
              <div class="field">
                <label>Nome do vendedor *</label>
                <input id="seller-name" required>
              </div>

              <div class="field">
                <label>Telefone</label>
                <input id="seller-phone">
              </div>

              <div class="field">
                <label>E-mail</label>
                <input id="seller-email" type="email">
              </div>

              <div class="field">
                <label>Meta mensal individual</label>
                <input id="seller-goal" type="number" min="0" step="0.01" value="0">
              </div>

              <div class="field">
                <label>Status</label>
                <select id="seller-status">
                  <option value="ativo">Ativo</option>
                  <option value="inativo">Inativo</option>
                </select>
              </div>
            </div>

            <div class="actions">
              <button class="button primary">Salvar vendedor</button>
            </div>
          </form>
        </div>

        <div class="panel">
          <h2>Vendedores cadastrados</h2>

          <div class="table-container">
            <table>
              <thead>
                <tr>
                  <th>Nome</th>
                  <th>Telefone</th>
                  <th>E-mail</th>
                  <th>Meta mensal</th>
                  <th>Faturamento</th>
                  <th>Status</th>
                  <th>Ações</th>
                </tr>
              </thead>
              <tbody id="sellers-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- FINANCEIRO -->
      <section class="page" id="page-financeiro">
        <div class="cards">
          <div class="card">
            <div class="metric-label">Contas a receber</div>
            <div class="metric-value green" id="finance-receivable">R$ 0,00</div>
          </div>

          <div class="card">
            <div class="metric-label">Contas a pagar</div>
            <div class="metric-value red" id="finance-payable">R$ 0,00</div>
          </div>

          <div class="card">
            <div class="metric-label">Recebido</div>
            <div class="metric-value blue" id="finance-received">R$ 0,00</div>
          </div>

          <div class="card">
            <div class="metric-label">Resultado DRE</div>
            <div class="metric-value purple" id="finance-result">R$ 0,00</div>
          </div>
        </div>

        <div class="panel">
          <h2>Nova movimentação financeira</h2>

          <form id="finance-form">
            <div class="grid-4">
              <div class="field">
                <label>Tipo *</label>
                <select id="finance-type">
                  <option value="receber">Conta a receber</option>
                  <option value="pagar">Conta a pagar</option>
                </select>
              </div>

              <div class="field">
                <label>Descrição *</label>
                <input id="finance-description" required>
              </div>

              <div class="field">
                <label>Valor *</label>
                <input id="finance-value" type="number" min="0" step="0.01" required>
              </div>

              <div class="field">
                <label>Vencimento *</label>
                <input id="finance-due" type="date" required>
              </div>

              <div class="field">
                <label>Status</label>
                <select id="finance-status">
                  <option value="pendente">Pendente</option>
                  <option value="pago">Pago</option>
                </select>
              </div>
            </div>

            <div class="actions">
              <button class="button primary">Salvar movimentação</button>
            </div>
          </form>
        </div>

        <div class="panel">
          <h2>Movimentações financeiras</h2>

          <div class="table-container">
            <table>
              <thead>
                <tr>
                  <th>Tipo</th>
                  <th>Descrição</th>
                  <th>Valor</th>
                  <th>Vencimento</th>
                  <th>Status</th>
                  <th>Ação</th>
                </tr>
              </thead>
              <tbody id="finance-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- CURVA ABC -->
      <section class="page" id="page-abc">
        <div class="panel">
          <div class="toolbar">
            <div>
              <h2>Curva ABC de produtos</h2>
              <div class="muted">
                Classificação automática pelo faturamento acumulado.
              </div>
            </div>

            <select id="abc-period" onchange="renderABC()">
              <option value="all">Todo o período</option>
              <option value="365">Últimos 365 dias</option>
              <option value="90">Últimos 90 dias</option>
              <option value="30">Últimos 30 dias</option>
            </select>
          </div>

          <div class="alert">
            <strong>Critério utilizado:</strong>
            Curva A representa até 60% do faturamento acumulado.
            Curva B representa de 60% até 90%.
            Curva C representa os 10% restantes.
          </div>

          <div class="chips" style="margin-bottom:14px">
            <span class="abc-big a">Curva A · 60%</span>
            <span class="abc-big b">Curva B · 30%</span>
            <span class="abc-big c">Curva C · 10%</span>
          </div>

          <div class="table-container">
            <table>
              <thead>
                <tr>
                  <th>Posição</th>
                  <th>Produto</th>
                  <th>Fornecedor</th>
                  <th>Curva</th>
                  <th>Quantidade</th>
                  <th>Faturamento</th>
                  <th>% individual</th>
                  <th>% acumulado</th>
                  <th>Clientes</th>
                </tr>
              </thead>
              <tbody id="abc-products-table"></tbody>
            </table>
          </div>
        </div>

        <div class="panel">
          <h2>Curva ABC de clientes</h2>

          <div class="table-container">
            <table>
              <thead>
                <tr>
                  <th>Cliente</th>
                  <th>Curva</th>
                  <th>Pedidos</th>
                  <th>Itens</th>
                  <th>Faturamento</th>
                  <th>% individual</th>
                  <th>% acumulado</th>
                  <th>Última compra</th>
                  <th>Ação</th>
                </tr>
              </thead>
              <tbody id="abc-clients-table"></tbody>
            </table>
          </div>
        </div>
      </section>

      <!-- PERFIL DO CLIENTE -->
      <section class="page" id="page-profile">
        <div id="client-profile"></div>
      </section>
    </main>
  </div>

  <!-- MODAL DE META -->
  <div class="modal" id="settings-modal">
    <div class="modal-content">
      <div class="modal-header">
        <h2>Configurar meta</h2>
        <button class="close" onclick="closeModal('settings-modal')">×</button>
      </div>

      <form id="settings-form">
        <div class="grid-3">
          <div class="field">
            <label>Meta mensal *</label>
            <input id="monthly-goal" type="number" min="0" step="0.01" required>
          </div>

          <div class="field">
            <label>Dias considerados *</label>
            <input id="considered-days" type="number" min="1" max="31" value="30" required>
          </div>

          <div class="field">
            <label>Meta diária calculada</label>
            <input id="daily-goal" type="number" readonly>
          </div>
        </div>

        <div class="alert">
          A meta diária será calculada automaticamente pela fórmula:
          meta mensal ÷ dias considerados.
        </div>

        <div class="actions">
          <button class="button primary">Salvar meta</button>
          <button type="button" class="button" onclick="closeModal('settings-modal')">
            Cancelar
          </button>
        </div>
      </form>
    </div>
  </div>

  <!-- MODAL DE VENDA -->
  <div class="modal" id="sale-modal">
    <div class="modal-content">
      <div class="modal-header">
        <h2>Nova venda</h2>
        <button class="close" onclick="closeModal('sale-modal')">×</button>
      </div>

      <form id="sale-form">
        <div class="grid-4">
          <div class="field">
            <label>Cliente *</label>
            <select id="sale-client" required></select>
          </div>

          <div class="field">
            <label>Vendedor *</label>
            <select id="sale-seller" required></select>
          </div>

          <div class="field">
            <label>Data *</label>
            <input id="sale-date" type="date" required>
          </div>

          <div class="field">
            <label>Canal</label>
            <select id="sale-channel">
              <option>Presencial</option>
              <option>WhatsApp</option>
              <option>Telefone</option>
              <option>Site</option>
              <option>Outro</option>
            </select>
          </div>
        </div>

        <h3 style="margin-top:20px">Itens da venda</h3>

        <div class="alert">
          Selecione o fornecedor antes do produto.
          O sistema exibirá apenas produtos vinculados ao fornecedor selecionado.
        </div>

        <div id="sale-lines"></div>

        <button type="button" class="button small" onclick="addSaleLine()">
          + Adicionar item
        </button>

        <div class="field" style="margin-top:15px">
          <label>Observações</label>
          <textarea id="sale-notes"></textarea>
        </div>

        <div style="margin-top:15px;text-align:right;font-size:19px">
          Total:
          <strong class="green" id="sale-total">R$ 0,00</strong>
        </div>

        <div class="actions">
          <button class="button primary">Salvar venda</button>
          <button type="button" class="button" onclick="closeModal('sale-modal')">
            Cancelar
          </button>
        </div>
      </form>
    </div>
  </div>

  <!-- MODAL DO PEDIDO -->
  <div class="modal" id="order-modal">
    <div class="modal-content">
      <div class="modal-header">
        <h2>Detalhes do pedido</h2>
        <button class="close" onclick="closeModal('order-modal')">×</button>
      </div>

      <div id="order-details"></div>
    </div>
  </div>

  <script>
    const STORAGE_KEY = "gestao_comercial_completo_2026";

    let database = JSON.parse(localStorage.getItem(STORAGE_KEY)) || {
      settings: {
        monthlyGoal: 0,
        dailyGoal: 0,
        consideredDays: 30
      },
      clients: [],
      suppliers: [],
      sellers: [],
      products: [],
      sales: [],
      finances: [],
      attachments: [],
      lowerReasons: []
    };

    database.settings = database.settings || {};
    database.settings.monthlyGoal = Number(database.settings.monthlyGoal || 0);
    database.settings.dailyGoal = Number(database.settings.dailyGoal || 0);
    database.settings.consideredDays = Number(database.settings.consideredDays || 30);

    if (!Array.isArray(database.clients)) database.clients = [];
    if (!Array.isArray(database.suppliers)) database.suppliers = [];
    if (!Array.isArray(database.sellers)) database.sellers = [];
    if (!Array.isArray(database.products)) database.products = [];
    if (!Array.isArray(database.sales)) database.sales = [];
    if (!Array.isArray(database.finances)) database.finances = [];
    if (!Array.isArray(database.attachments)) database.attachments = [];
    if (!Array.isArray(database.lowerReasons)) database.lowerReasons = [];

    saveDatabase();

    function saveDatabase() {
      localStorage.setItem(STORAGE_KEY, JSON.stringify(database));
    }

    function createId(prefix) {
      return prefix + "_" + Date.now().toString(36) +
        Math.random().toString(36).substring(2, 8);
    }

    function today() {
      return new Date().toISOString().substring(0, 10);
    }

    function money(value) {
      return Number(value || 0).toLocaleString("pt-BR", {
        style: "currency",
        currency: "BRL"
      });
    }

    function dateBR(value) {
      if (!value) return "—";

      const parts = String(value).split("-");

      if (parts.length !== 3) return value;

      return parts[2] + "/" + parts[1] + "/" + parts[0];
    }

    function escapeHTML(value) {
      return String(value ?? "").replace(/[&<>"']/g, function(character) {
        const replacements = {
          "&": "&",
          "<": "<",
          ">": ">",
          '"': "&quot;",
          "'": "&#039;"
        };

        return replacements[character];
      });
    }

    function getClient(clientId) {
      return database.clients.find(function(client) {
        return client.id === clientId;
      });
    }

    function getSupplier(supplierId) {
      return database.suppliers.find(function(supplier) {
        return supplier.id === supplierId;
      });
    }

    function getSeller(sellerId) {
      return database.sellers.find(function(seller) {
        return seller.id === sellerId;
      });
    }

    function getProduct(productId) {
      return database.products.find(function(product) {
        return product.id === productId;
      });
    }

    function getSaleTotal(sale) {
      return (sale.items || []).reduce(function(total, item) {
        return total + Number(item.quantity || 0) * Number(item.price || 0);
      }, 0);
    }

    function getClientSales(clientId, source) {
      return (source || database.sales).filter(function(sale) {
        return sale.clientId === clientId;
      });
    }

    function getProductQuantity(productId, source) {
      return (source || database.sales).reduce(function(total, sale) {
        return total + (sale.items || []).reduce(function(sum, item) {
          return sum + (
            item.productId === productId
              ? Number(item.quantity || 0)
              : 0
          );
        }, 0);
      }, 0);
    }

    function getProductRevenue(productId, source) {
      return (source || database.sales).reduce(function(total, sale) {
        return total + (sale.items || []).reduce(function(sum, item) {
          if (item.productId !== productId) return sum;

          return sum + Number(item.quantity || 0) * Number(item.price || 0);
        }, 0);
      }, 0);
    }

    function getProductClients(productId, source) {
      const clients = [];

      (source || database.sales).forEach(function(sale) {
        const hasProduct = (sale.items || []).some(function(item) {
          return item.productId === productId;
        });

        if (hasProduct && !clients.includes(sale.clientId)) {
          clients.push(sale.clientId);
        }
      });

      return clients.length;
    }

    function getClientStats(clientId, source) {
      const sales = getClientSales(clientId, source);
      const quantities = {};
      let revenue = 0;
      let items = 0;

      sales.forEach(function(sale) {
        revenue += getSaleTotal(sale);

        (sale.items || []).forEach(function(item) {
          quantities[item.productId] =
            (quantities[item.productId] || 0) +
            Number(item.quantity || 0);

          items += Number(item.quantity || 0);
        });
      });

      const dates = sales
        .map(function(sale) {
          return sale.date;
        })
        .filter(Boolean)
        .sort()
        .reverse();

      return {
        sales: sales,
        quantities: quantities,
        revenue: revenue,
        items: items,
        lastSale: dates[0] || ""
      };
    }

    function getDaysWithoutPurchase(client) {
      const stats = getClientStats(client.id);

      if (!stats.lastSale) return Infinity;

      const lastDate = new Date(stats.lastSale + "T12:00:00");

      return Math.floor((new Date() - lastDate) / 86400000);
    }

    function getClientStatus(client) {
      const days = getDaysWithoutPurchase(client);

      if (days === Infinity) return "Nunca comprou";
      if (days > 45) return "Mais de 45 dias";
      if (days > 30) return "Mais de 30 dias";
      if (days > 15) return "Mais de 15 dias";

      return "Ativo";
    }

    function getMonthSales() {
      const month = today().substring(0, 7);

      return database.sales.filter(function(sale) {
        return String(sale.date).substring(0, 7) === month;
      });
    }

    function getRemainingDaysInMonth() {
      const current = new Date();

      return new Date(
        current.getFullYear(),
        current.getMonth() + 1,
        0
      ).getDate() - current.getDate() + 1;
    }

    function supplierChip(supplier, active) {
      if (!supplier) return "";

      return `
        <span class="chip ${active === false ? "inactive" : ""}">
          <span
            class="dot"
            style="background:${active === false ? "#555" : supplier.color}">
          </span>
          ${escapeHTML(supplier.name)}
        </span>
      `;
    }

    function abcBadge(curve) {
      const normalized = String(curve).toLowerCase();

      return `
        <span class="badge badge-${normalized}">
          Curva ${String(curve).toUpperCase()}
        </span>
      `;
    }

    function showPage(page) {
      document.querySelectorAll(".page").forEach(function(section) {
        section.classList.remove("active");
      });

      document.querySelectorAll(".nav-button").forEach(function(button) {
        button.classList.remove("active");
      });

      const pageElement = document.getElementById("page-" + page);

      if (pageElement) {
        pageElement.classList.add("active");
      }

      const nav = document.querySelector('[data-page="' + page + '"]');

      if (nav) {
        nav.classList.add("active");
      }

      const titles = {
        dashboard: "Dashboard",
        clientes: "Clientes",
        produtos: "Produtos",
        fornecedores: "Fornecedores",
        vendedores: "Vendedores",
        financeiro: "Financeiro",
        abc: "Curva ABC",
        profile: "Perfil do cliente"
      };

      document.getElementById("page-title").textContent =
        titles[page] || "Gestão";
    }

    document.querySelectorAll(".nav-button").forEach(function(button) {
      button.addEventListener("click", function() {
        showPage(button.dataset.page);
        renderAll();
      });
    });

    function renderAll() {
      renderDashboard();
      renderClients();
      renderProducts();
      renderSuppliers();
      renderSellers();
      renderFinance();
      renderABC();
      updateSelects();
    }

    function renderDashboard() {
      const totalRevenue = database.sales.reduce(function(total, sale) {
        return total + getSaleTotal(sale);
      }, 0);

      const monthRevenue = getMonthSales().reduce(function(total, sale) {
        return total + getSaleTotal(sale);
      }, 0);

      const monthlyGoal = Number(database.settings.monthlyGoal || 0);
      const consideredDays = Number(database.settings.consideredDays || 30);
      const dailyGoal = monthlyGoal / Math.max(consideredDays, 1);
      const missing = Math.max(monthlyGoal - monthRevenue, 0);
      const remainingDays = getRemainingDaysInMonth();
      const necessaryDaily = missing / Math.max(remainingDays, 1);
      const progress = monthlyGoal > 0
        ? Math.min(monthRevenue / monthlyGoal * 100, 100)
        : 0;

      document.getElementById("goal-month").textContent = money(monthlyGoal);
      document.getElementById("goal-daily").textContent = money(dailyGoal);
      document.getElementById("goal-sold").textContent = money(monthRevenue);
      document.getElementById("goal-missing").textContent = money(missing);
      document.getElementById("goal-progress").style.width = progress + "%";

      document.getElementById("goal-summary").textContent =
        "Meta diária: " + money(dailyGoal) +
        " · Necessário por dia até o fim do mês: " +
        money(necessaryDaily) +
        " · Dias considerados: " + consideredDays +
        " · " + progress.toFixed(1) +
        "% da meta atingida.";

      document.getElementById("metric-clients").textContent =
        database.clients.length;

      document.getElementById("metric-products").textContent =
        database.products.length;

      document.getElementById("metric-sales").textContent =
        database.sales.length;

      document.getElementById("metric-revenue").textContent =
        money(totalRevenue);

      renderBirthdays();
      renderInactive();
      renderExpansion();
      renderUnusedProducts();

      const alerts = [];

      if (monthlyGoal <= 0) {
        alerts.push(`
          <div class="alert">
            A meta mensal ainda não foi configurada.
            Clique em <strong>Configurar meta</strong>.
          </div>
        `);
      }

      const warranties = getWarrantyPendencies();

      if (warranties.length) {
        alerts.push(`
          <div class="alert red-alert">
            Existem <strong>${warranties.length}</strong>
            garantia(s) ativa(s) para acompanhamento.
          </div>
        `);
      }

      document.getElementById("dashboard-alerts").innerHTML =
        alerts.join("");
    }

    function renderBirthdays() {
      const currentMonth = today().substring(5, 7);

      const birthdays = database.clients
        .filter(function(client) {
          return client.birth &&
            client.birth.substring(5, 7) === currentMonth;
        })
        .sort(function(a, b) {
          return a.birth.substring(8, 10)
            .localeCompare(b.birth.substring(8, 10));
        });

      document.getElementById("birthdays-list").innerHTML =
        birthdays.length
          ? birthdays.map(function(client) {
              return `
                <div
                  class="list-item"
                  style="cursor:pointer"
                  onclick="openClientProfile('${client.id}')">

                  <strong>${escapeHTML(client.name)}</strong>

                  <div class="muted">
                    Aniversário: dia ${client.birth.substring(8, 10)}
                    · ${escapeHTML(client.phone || "Sem telefone")}
                  </div>

                  <div class="actions">
                    <button
                      class="button small success"
                      onclick="event.stopPropagation();sendBirthday('${client.id}')">
                      Preparar WhatsApp
                    </button>
                  </div>
                </div>
              `;
            }).join("")
          : `<div class="empty">Nenhum aniversariante neste mês.</div>`;
    }

    function renderInactive() {
      const inactive = database.clients
        .map(function(client) {
          return {
            client: client,
            days: getDaysWithoutPurchase(client),
            stats: getClientStats(client.id)
          };
        })
        .filter(function(item) {
          return item.days === Infinity || item.days > 15;
        })
        .sort(function(a, b) {
          if (a.days === Infinity) return -1;
          if (b.days === Infinity) return 1;

          return b.days - a.days;
        });

      document.getElementById("inactive-list").innerHTML =
        inactive.length
          ? inactive.map(function(item) {
              return `
                <div
                  class="list-item"
                  style="cursor:pointer"
                  onclick="openClientProfile('${item.client.id}')">

                  <strong>${escapeHTML(item.client.name)}</strong>

                  <div class="muted">
                    ${
                      item.days === Infinity
                        ? "Nunca comprou"
                        : item.days + " dia(s) sem comprar"
                    }
                    · Faturamento: ${money(item.stats.revenue)}
                  </div>
                </div>
              `;
            }).join("")
          : `<div class="empty">Nenhum cliente inativo.</div>`;
    }

    function renderExpansion() {
      const opportunities = database.clients
        .map(function(client) {
          const stats = getClientStats(client.id);
          const suggestions = getSuggestions(client.id);
          const lower = getLowerPurchases(client.id);

          return {
            client: client,
            stats: stats,
            suggestions: suggestions,
            lower: lower
          };
        })
        .filter(function(item) {
          return item.suggestions.length || item.lower.length;
        })
        .slice(0, 10);

      document.getElementById("expansion-list").innerHTML =
        opportunities.length
          ? opportunities.map(function(item) {
              const suggestionNames = item.suggestions
                .slice(0, 3)
                .map(function(suggestion) {
                  return suggestion.product.name;
                })
                .join(", ");

              const lowerNames = item.lower
                .slice(0, 2)
                .map(function(item) {
                  return item.product.name;
                })
                .join(", ");

              return `
                <div
                  class="list-item"
                  style="cursor:pointer"
                  onclick="openClientProfile('${item.client.id}')">

                  <strong>${escapeHTML(item.client.name)}</strong>

                  <div class="muted">
                    ${item.stats.sales.length} pedido(s)
                    · ${money(item.stats.revenue)}
                  </div>

                  ${
                    suggestionNames
                      ? `
                        <div class="muted" style="margin-top:5px">
                          Sugestões: ${escapeHTML(suggestionNames)}
                        </div>
                      `
                      : ""
                  }

                  ${
                    lowerNames
                      ? `
                        <div class="muted" style="margin-top:5px">
                          Abaixo da média: ${escapeHTML(lowerNames)}
                        </div>
                      `
                      : ""
                  }
                </div>
              `;
            }).join("")
          : `<div class="empty">Nenhuma oportunidade identificada.</div>`;
    }

    function renderUnusedProducts() {
      const unused = database.products.filter(function(product) {
        return getProductQuantity(product.id) === 0;
      });

      document.getElementById("unused-products").innerHTML =
        unused.length
          ? unused.map(function(product) {
              const supplier = getSupplier(product.supplierId);

              return `
                <div class="list-item">
                  <strong>${escapeHTML(product.name)}</strong>

                  <div class="muted">
                    SKU: ${escapeHTML(product.sku)}
                    · ${escapeHTML(supplier?.name || "Sem fornecedor")}
                  </div>
                </div>
              `;
            }).join("")
          : `<div class="empty">Todos os produtos possuem pedidos.</div>`;
    }

    function renderClients() {
      const search = (
        document.getElementById("client-search")?.value || ""
      ).toLowerCase();

      const clients = database.clients.filter(function(client) {
        return client.name.toLowerCase().includes(search) ||
          (client.phone || "").toLowerCase().includes(search) ||
          (client.email || "").toLowerCase().includes(search);
      });

      document.getElementById("clients-table").innerHTML =
        clients.length
          ? clients.map(function(client) {
              const stats = getClientStats(client.id);
              const status = getClientStatus(client);
              const statusClass = status === "Ativo"
                ? "badge-active"
                : "badge-inactive";

              return `
                <tr
                  class="clickable"
                  onclick="openClientProfile('${client.id}')">

                  <td>
                    <strong>${escapeHTML(client.name)}</strong>
                    <br>
                    <span class="muted">
                      ${escapeHTML(client.city || "")}
                    </span>
                  </td>

                  <td>
                    ${escapeHTML(client.phone || "—")}
                    <br>
                    <span class="muted">
                      ${escapeHTML(client.email || "")}
                    </span>
                  </td>

                  <td>${dateBR(stats.lastSale)}</td>

                  <td>
                    <span class="badge ${statusClass}">
                      ${status}
                    </span>
                  </td>

                  <td>${stats.sales.length}</td>
                  <td class="green">${money(stats.revenue)}</td>

                  <td>
                    <button
                      class="button small"
                      onclick="event.stopPropagation();openClientProfile('${client.id}')">
                      Abrir
                    </button>

                    <button
                      class="button small danger"
                      onclick="event.stopPropagation();deleteClient('${client.id}')">
                      Excluir
                    </button>
                  </td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="7" class="empty">
                Nenhum cliente encontrado.
              </td>
            </tr>
          `;
    }

    document.getElementById("client-form").addEventListener("submit", function(event) {
      event.preventDefault();

      database.clients.push({
        id: createId("client"),
        name: document.getElementById("client-name").value.trim(),
        phone: document.getElementById("client-phone").value.trim(),
        email: document.getElementById("client-email").value.trim(),
        birth: document.getElementById("client-birth").value,
        city: document.getElementById("client-city").value.trim(),
        notes: document.getElementById("client-notes").value.trim(),
        createdAt: today()
      });

      saveDatabase();
      event.target.reset();
      renderAll();

      alert("Cliente cadastrado com sucesso.");
    });

    function deleteClient(clientId) {
      const client = getClient(clientId);

      if (!client) return;

      if (!confirm("Excluir o cliente e seu histórico de vendas?")) return;

      database.clients = database.clients.filter(function(item) {
        return item.id !== clientId;
      });

      database.sales = database.sales.filter(function(sale) {
        return sale.clientId !== clientId;
      });

      database.attachments = database.attachments.filter(function(file) {
        return file.clientId !== clientId;
      });

      database.lowerReasons = database.lowerReasons.filter(function(item) {
        return item.clientId !== clientId;
      });

      saveDatabase();
      renderAll();
    }

    function renderSuppliers() {
      document.getElementById("suppliers-table").innerHTML =
        database.suppliers.length
          ? database.suppliers.map(function(supplier) {
              const products = database.products.filter(function(product) {
                return product.supplierId === supplier.id;
              });

              return `
                <tr>
                  <td>
                    ${supplierChip(supplier, true)}
                  </td>

                  <td>${escapeHTML(supplier.contact || "—")}</td>

                  <td>
                    ${
                      products.length
                        ? products.map(function(product) {
                            return `
                              <div class="muted">
                                ${escapeHTML(product.sku)}
                                — ${escapeHTML(product.name)}
                              </div>
                            `;
                          }).join("")
                        : "Nenhum produto"
                    }
                  </td>

                  <td>
                    <button
                      class="button small danger"
                      onclick="deleteSupplier('${supplier.id}')">
                      Excluir
                    </button>
                  </td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="4" class="empty">
                Nenhum fornecedor cadastrado.
              </td>
            </tr>
          `;
    }

    document.getElementById("supplier-form").addEventListener("submit", function(event) {
      event.preventDefault();

      database.suppliers.push({
        id: createId("supplier"),
        name: document.getElementById("supplier-name").value.trim(),
        contact: document.getElementById("supplier-contact").value.trim(),
        color: document.getElementById("supplier-color").value
      });

      saveDatabase();
      event.target.reset();
      document.getElementById("supplier-color").value = "#e50914";
      renderAll();

      alert("Fornecedor cadastrado com sucesso.");
    });

    function deleteSupplier(supplierId) {
      const linked = database.products.some(function(product) {
        return product.supplierId === supplierId;
      });

      if (linked) {
        alert("Não é possível excluir fornecedor com produtos vinculados.");
        return;
      }

      database.suppliers = database.suppliers.filter(function(supplier) {
        return supplier.id !== supplierId;
      });

      saveDatabase();
      renderAll();
    }

    function renderProducts() {
      const search = (
        document.getElementById("product-search")?.value || ""
      ).toLowerCase();

      const productRows = database.products.map(function(product) {
        return {
          product: product,
          revenue: getProductRevenue(product.id)
        };
      });

      const abc = calculateABC(productRows);

      const products = database.products.filter(function(product) {
        return product.name.toLowerCase().includes(search) ||
          product.sku.toLowerCase().includes(search) ||
          (product.category || "").toLowerCase().includes(search);
      });

      document.getElementById("products-table").innerHTML =
        products.length
          ? products.map(function(product) {
              const supplier = getSupplier(product.supplierId);
              const classification = abc.find(function(item) {
                return item.row.product.id === product.id;
              });

              const curve = classification?.curve || "C";

              return `
                <tr class="abc-row-${curve.toLowerCase()}">
                  <td>
                    <strong>${escapeHTML(product.sku)}</strong>
                  </td>

                  <td>
                    <strong>${escapeHTML(product.name)}</strong>
                    <br>
                    <span class="muted">
                      Garantia: ${product.warrantyDays || 0} dia(s)
                    </span>
                  </td>

                  <td>
                    ${supplier ? supplierChip(supplier, true) : "—"}
                  </td>

                  <td>${escapeHTML(product.category || "—")}</td>
                  <td>${money(product.price)}</td>
                  <td>${abcBadge(curve)}</td>
                  <td>${getProductQuantity(product.id)}</td>

                  <td>
                    <button
                      class="button small danger"
                      onclick="deleteProduct('${product.id}')">
                      Excluir
                    </button>
                  </td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="8" class="empty">
                Nenhum produto encontrado.
              </td>
            </tr>
          `;
    }

    document.getElementById("product-form").addEventListener("submit", function(event) {
      event.preventDefault();

      const sku = document
        .getElementById("product-sku")
        .value
        .trim()
        .toUpperCase();

      const exists = database.products.some(function(product) {
        return product.sku.toUpperCase() === sku;
      });

      if (exists) {
        alert("Este SKU já está cadastrado.");
        return;
      }

      const supplierId = document.getElementById("product-supplier").value;

      if (!supplierId) {
        alert("Selecione o fornecedor.");
        return;
      }

      database.products.push({
        id: createId("product"),
        sku: sku,
        name: document.getElementById("product-name").value.trim(),
        supplierId: supplierId,
        price: Number(document.getElementById("product-price").value || 0),
        category: document.getElementById("product-category").value.trim(),
        warrantyDays: Number(
          document.getElementById("product-warranty").value || 0
        ),
        notes: document.getElementById("product-notes").value.trim()
      });

      saveDatabase();
      event.target.reset();
      renderAll();

      alert("Produto cadastrado com sucesso.");
    });

    function deleteProduct(productId) {
      const used = database.sales.some(function(sale) {
        return (sale.items || []).some(function(item) {
          return item.productId === productId;
        });
      });

      if (used) {
        alert("Produto com histórico de vendas não pode ser excluído.");
        return;
      }

      database.products = database.products.filter(function(product) {
        return product.id !== productId;
      });

      saveDatabase();
      renderAll();
    }

    document.getElementById("seller-form").addEventListener("submit", function(event) {
      event.preventDefault();

      database.sellers.push({
        id: createId("seller"),
        name: document.getElementById("seller-name").value.trim(),
        phone: document.getElementById("seller-phone").value.trim(),
        email: document.getElementById("seller-email").value.trim(),
        monthlyGoal: Number(
          document.getElementById("seller-goal").value || 0
        ),
        status: document.getElementById("seller-status").value,
        createdAt: today()
      });

      saveDatabase();
      event.target.reset();
      renderAll();

      alert("Vendedor cadastrado com sucesso.");
    });

    function getSellerRevenue(sellerId) {
      return database.sales
        .filter(function(sale) {
          return sale.sellerId === sellerId;
        })
        .reduce(function(total, sale) {
          return total + getSaleTotal(sale);
        }, 0);
    }

    function renderSellers() {
      document.getElementById("sellers-table").innerHTML =
        database.sellers.length
          ? database.sellers.map(function(seller) {
              return `
                <tr>
                  <td><strong>${escapeHTML(seller.name)}</strong></td>
                  <td>${escapeHTML(seller.phone || "—")}</td>
                  <td>${escapeHTML(seller.email || "—")}</td>
                  <td>${money(seller.monthlyGoal)}</td>
                  <td class="green">${money(getSellerRevenue(seller.id))}</td>
                  <td>
                    <span class="badge ${
                      seller.status === "ativo"
                        ? "badge-active"
                        : "badge-inactive"
                    }">
                      ${seller.status === "ativo" ? "Ativo" : "Inativo"}
                    </span>
                  </td>
                  <td>
                    <button
                      class="button small danger"
                      onclick="deleteSeller('${seller.id}')">
                      Excluir
                    </button>
                  </td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="7" class="empty">
                Nenhum vendedor cadastrado.
              </td>
            </tr>
          `;
    }

    function deleteSeller(sellerId) {
      const used = database.sales.some(function(sale) {
        return sale.sellerId === sellerId;
      });

      if (used) {
        alert("Vendedor com vendas registradas não pode ser excluído.");
        return;
      }

      database.sellers = database.sellers.filter(function(seller) {
        return seller.id !== sellerId;
      });

      saveDatabase();
      renderAll();
    }

    function updateSelects() {
      const supplierSelect = document.getElementById("product-supplier");

      if (supplierSelect) {
        supplierSelect.innerHTML =
          `<option value="">Selecione...</option>` +
          database.suppliers.map(function(supplier) {
            return `
              <option value="${supplier.id}">
                ${escapeHTML(supplier.name)}
              </option>
            `;
          }).join("");
      }

      const clientSelect = document.getElementById("sale-client");

      if (clientSelect) {
        clientSelect.innerHTML =
          `<option value="">Selecione...</option>` +
          database.clients.map(function(client) {
            return `
              <option value="${client.id}">
                ${escapeHTML(client.name)}
              </option>
            `;
          }).join("");
      }

      const sellerSelect = document.getElementById("sale-seller");

      if (sellerSelect) {
        sellerSelect.innerHTML =
          `<option value="">Selecione...</option>` +
          database.sellers
            .filter(function(seller) {
              return seller.status !== "inativo";
            })
            .map(function(seller) {
              return `
                <option value="${seller.id}">
                  ${escapeHTML(seller.name)}
                </option>
              `;
            }).join("");
      }
    }

    function calculateDailyGoal() {
      const monthly = Number(
        document.getElementById("monthly-goal").value || 0
      );

      const days = Number(
        document.getElementById("considered-days").value || 1
      );

      document.getElementById("daily-goal").value =
        (monthly / Math.max(days, 1)).toFixed(2);
    }

    document.getElementById("monthly-goal").addEventListener(
      "input",
      calculateDailyGoal
    );

    document.getElementById("considered-days").addEventListener(
      "input",
      calculateDailyGoal
    );

    function openSettingsModal() {
      document.getElementById("monthly-goal").value =
        database.settings.monthlyGoal || "";

      document.getElementById("considered-days").value =
        database.settings.consideredDays || 30;

      calculateDailyGoal();

      document.getElementById("settings-modal").classList.add("open");
    }

    document.getElementById("settings-form").addEventListener("submit", function(event) {
      event.preventDefault();

      const monthly = Number(
        document.getElementById("monthly-goal").value || 0
      );

      const days = Number(
        document.getElementById("considered-days").value || 1
      );

      const daily = monthly / Math.max(days, 1);

      database.settings.monthlyGoal = monthly;
      database.settings.consideredDays = days;
      database.settings.dailyGoal = daily;

      saveDatabase();
      closeModal("settings-modal");
      renderAll();

      alert("Meta mensal salva e meta diária calculada automaticamente.");
    });

    function openSaleModal(clientId) {
      updateSelects();

      document.getElementById("sale-client").value = clientId || "";
      document.getElementById("sale-seller").value = "";
      document.getElementById("sale-date").value = today();
      document.getElementById("sale-notes").value = "";
      document.getElementById("sale-lines").innerHTML = "";

      addSaleLine();

      document.getElementById("sale-modal").classList.add("open");
    }

    function addSaleLine() {
      const line = document.createElement("div");

      line.className = "sale-line";

      line.innerHTML = `
        <div class="field supplier-field">
          <label>Fornecedor *</label>

          <select class="sale-supplier" onchange="updateLineProducts(this)">
            <option value="">Selecione...</option>

            ${database.suppliers.map(function(supplier) {
              return `
                <option value="${supplier.id}">
                  ${escapeHTML(supplier.name)}
                </option>
              `;
            }).join("")}
          </select>
        </div>

        <div class="field product-field">
          <label>Produto / SKU *</label>

          <select class="sale-product" onchange="updateSaleTotal()" disabled>
            <option value="">Selecione o fornecedor...</option>
          </select>
        </div>

        <div class="field">
          <label>Quantidade</label>

          <input
            class="sale-quantity"
            type="number"
            min="1"
            value="1"
            oninput="updateSaleTotal()">
        </div>

        <div class="line-total">R$ 0,00</div>

        <button
          type="button"
          class="button small danger"
          onclick="this.parentElement.remove();updateSaleTotal()">
          ×
        </button>
      `;

      document.getElementById("sale-lines").appendChild(line);
      updateSaleTotal();
    }

    function updateLineProducts(supplierSelect) {
      const line = supplierSelect.closest(".sale-line");
      const productSelect = line.querySelector(".sale-product");
      const supplierId = supplierSelect.value;

      const products = database.products.filter(function(product) {
        return product.supplierId === supplierId;
      });

      productSelect.disabled = !supplierId;

      productSelect.innerHTML = supplierId
        ? `
          <option value="">Selecione o produto...</option>
          ${products.map(function(product) {
            return `
              <option value="${product.id}">
                ${escapeHTML(product.sku)}
                — ${escapeHTML(product.name)}
                (${money(product.price)})
              </option>
            `;
          }).join("")}
        `
        : `<option value="">Selecione o fornecedor...</option>`;

      updateSaleTotal();
    }

    function updateSaleTotal() {
      let total = 0;

      document.querySelectorAll(".sale-line").forEach(function(line) {
        const product = getProduct(
          line.querySelector(".sale-product")?.value
        );

        const quantity = Number(
          line.querySelector(".sale-quantity")?.value || 0
        );

        const lineTotal = product
          ? product.price * quantity
          : 0;

        total += lineTotal;

        const display = line.querySelector(".line-total");

        if (display) {
          display.textContent = money(lineTotal);
        }
      });

      document.getElementById("sale-total").textContent = money(total);
    }

    document.getElementById("sale-form").addEventListener("submit", function(event) {
      event.preventDefault();

      const clientId = document.getElementById("sale-client").value;
      const sellerId = document.getElementById("sale-seller").value;
      const items = [];
      let invalid = false;

      document.querySelectorAll(".sale-line").forEach(function(line) {
        const supplierId = line.querySelector(".sale-supplier").value;
        const productId = line.querySelector(".sale-product").value;
        const quantity = Number(
          line.querySelector(".sale-quantity").value || 0
        );

        const product = getProduct(productId);

        if (!supplierId || !product || quantity <= 0) {
          invalid = true;
          return;
        }

        if (product.supplierId !== supplierId) {
          invalid = true;
          return;
        }

        items.push({
          productId: product.id,
          supplierId: supplierId,
          sku: product.sku,
          quantity: quantity,
          price: product.price,
          warrantyActive: false,
          warrantyStart: "",
          warrantyEnd: ""
        });
      });

      if (!clientId) {
        alert("Selecione o cliente.");
        return;
      }

      if (!sellerId) {
        alert("Selecione o vendedor.");
        return;
      }

      if (invalid || !items.length) {
        alert("Preencha corretamente todos os itens da venda.");
        return;
      }

      database.sales.push({
        id: createId("sale"),
        clientId: clientId,
        sellerId: sellerId,
        date: document.getElementById("sale-date").value,
        channel: document.getElementById("sale-channel").value,
        notes: document.getElementById("sale-notes").value.trim(),
        items: items
      });

      saveDatabase();
      closeModal("sale-modal");
      renderAll();

      alert("Venda registrada com sucesso.");
    });

    function getSalesByPeriod() {
      const period = document.getElementById("abc-period")?.value || "all";

      if (period === "all") {
        return database.sales;
      }

      const limit = new Date();

      limit.setDate(limit.getDate() - Number(period));

      return database.sales.filter(function(sale) {
        return new Date(sale.date + "T12:00:00") >= limit;
      });
    }

    /*
      REGRA DA CURVA ABC:

      - Os registros são ordenados pelo maior faturamento.
      - O percentual individual é calculado sobre o faturamento total.
      - O percentual acumulado define a curva.
      - Até 60%: Curva A.
      - Acima de 60% até 90%: Curva B.
      - Acima de 90%: Curva C.
      */
    function calculateABC(rows) {
      const sorted = rows.slice().sort(function(a, b) {
        return Number(b.revenue || 0) - Number(a.revenue || 0);
      });

      const total = sorted.reduce(function(sum, row) {
        return sum + Number(row.revenue || 0);
      }, 0);

      let accumulated = 0;

      return sorted.map(function(row, index) {
        const revenue = Number(row.revenue || 0);

        if (total <= 0 || revenue <= 0) {
          return {
            row: row,
            index: index + 1,
            individualPercentage: 0,
            accumulatedPercentage: 0,
            curve: "C"
          };
        }

        const individual = revenue / total * 100;

        accumulated += individual;

        let curve = "C";

        if (accumulated <= 60) {
          curve = "A";
        } else if (accumulated <= 90) {
          curve = "B";
        }

        return {
          row: row,
          index: index + 1,
          individualPercentage: individual,
          accumulatedPercentage: accumulated,
          curve: curve
        };
      });
    }

    function renderABC() {
      const source = getSalesByPeriod();

      const productRows = database.products.map(function(product) {
        return {
          product: product,
          revenue: getProductRevenue(product.id, source),
          quantity: getProductQuantity(product.id, source),
          clients: getProductClients(product.id, source)
        };
      });

      const productsABC = calculateABC(productRows);

      document.getElementById("abc-products-table").innerHTML =
        productsABC.length
          ? productsABC.map(function(item) {
              const product = item.row.product;
              const supplier = getSupplier(product.supplierId);

              return `
                <tr class="abc-row-${item.curve.toLowerCase()}">
                  <td>${item.index}</td>

                  <td>
                    <strong>${escapeHTML(product.name)}</strong>
                    <br>
                    <span class="muted">
                      SKU: ${escapeHTML(product.sku)}
                    </span>
                  </td>

                  <td>
                    ${supplier ? supplierChip(supplier, true) : "—"}
                  </td>

                  <td>${abcBadge(item.curve)}</td>
                  <td>${item.row.quantity}</td>
                  <td class="green">${money(item.row.revenue)}</td>
                  <td>${item.individualPercentage.toFixed(2)}%</td>
                  <td>${item.accumulatedPercentage.toFixed(2)}%</td>
                  <td>${item.row.clients}</td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="9" class="empty">
                Cadastre produtos e vendas para calcular a Curva ABC.
              </td>
            </tr>
          `;

      const clientRows = database.clients.map(function(client) {
        const stats = getClientStats(client.id, source);

        return {
          client: client,
          revenue: stats.revenue,
          stats: stats
        };
      });

      const clientsABC = calculateABC(clientRows);

      document.getElementById("abc-clients-table").innerHTML =
        clientsABC.length
          ? clientsABC.map(function(item) {
              const client = item.row.client;

              return `
                <tr
                  class="clickable abc-row-${item.curve.toLowerCase()}"
                  onclick="openClientProfile('${client.id}')">

                  <td>
                    <strong>${escapeHTML(client.name)}</strong>
                  </td>

                  <td>${abcBadge(item.curve)}</td>
                  <td>${item.row.stats.sales.length}</td>
                  <td>${item.row.stats.items}</td>
                  <td class="green">${money(item.row.revenue)}</td>
                  <td>${item.individualPercentage.toFixed(2)}%</td>
                  <td>${item.accumulatedPercentage.toFixed(2)}%</td>
                  <td>${dateBR(item.row.stats.lastSale)}</td>

                  <td>
                    <button
                      class="button small primary"
                      onclick="event.stopPropagation();openClientProfile('${client.id}')">
                      Ver perfil
                    </button>
                  </td>
                </tr>
              `;
            }).join("")
          : `
            <tr>
              <td colspan="9" class="empty">
                Cadastre clientes e vendas para calcular a Curva ABC.
              </td>
            </tr>
          `;
    }

    function getSuggestions(clientId) {
      const clientStats = getClientStats(clientId);
      const purchased = Object.keys(clientStats.quantities);

      const rows = database.products.map(function(product) {
        return {
          product: product,
          revenue: getProductRevenue(product.id),
          curve: calculateABC(
            database.products.map(function(item) {
              return {
                product: item,
                revenue: getProductRevenue(item.id)
              };
            })
          ).find(function(item) {
            return item.row.product.id === product.id;
          })?.curve || "C"
        };
      });

      const order = {
        A: 1,
        B: 2,
        C: 3
      };

      return rows
        .filter(function(item) {
          return !purchased.includes(item.product.id);
        })
        .sort(function(a, b) {
          return order[a.curve] - order[b.curve] ||
            b.revenue - a.revenue;
        });
    }

    function getLowerPurchases(clientId) {
      const clientStats = getClientStats(clientId);
      const result = [];

      database.products.forEach(function(product) {
        const clientQuantity = Number(
          clientStats.quantities[product.id] || 0
        );

        if (clientQuantity <= 0) return;

        let total = 0;
        let buyers = 0;

        database.clients.forEach(function(client) {
          const stats = getClientStats(client.id);
          const quantity = Number(stats.quantities[product.id] || 0);

          if (quantity > 0) {
            total += quantity;
            buyers++;
          }
        });

        if (!buyers) return;

        const average = total / buyers;

        if (clientQuantity < average) {
          const reason = database.lowerReasons.find(function(item) {
            return item.clientId === clientId &&
              item.productId === product.id;
          });

          result.push({
            product: product,
            clientQuantity: clientQuantity,
            average: average,
            reason: reason?.reason || ""
          });
        }
      });

      return result;
    }

    function openClientProfile(clientId) {
      const client = getClient(clientId);

      if (!client) return;

      const stats = getClientStats(clientId);
      const purchasedSuppliers = [];

      Object.keys(stats.quantities).forEach(function(productId) {
        const product = getProduct(productId);

        if (product && !purchasedSuppliers.includes(product.supplierId)) {
          purchasedSuppliers.push(product.supplierId);
        }
      });

      const suppliersHTML = database.suppliers.length
        ? database.suppliers.map(function(supplier) {
            return supplierChip(
              supplier,
              purchasedSuppliers.includes(supplier.id)
            );
          }).join("")
        : `<span class="muted">Nenhum fornecedor cadastrado.</span>`;

      const ordersHTML = stats.sales.length
        ? stats.sales
            .slice()
            .sort(function(a, b) {
              return b.date.localeCompare(a.date);
            })
            .map(function(sale) {
              return `
                <div class="list-item">
                  <strong>
                    Pedido de ${dateBR(sale.date)}
                    · ${money(getSaleTotal(sale))}
                  </strong>

                  <div class="muted">
                    Vendedor:
                    ${escapeHTML(getSeller(sale.sellerId)?.name || "—")}
                    · ${escapeHTML(sale.channel || "—")}
                  </div>

                  <div class="actions">
                    <button
                      class="button small"
                      onclick="openOrder('${sale.id}')">
                      Ver pedido
                    </button>

                    <button
                      class="button small primary"
                      onclick="downloadPDF('${sale.id}')">
                      Baixar PDF
                    </button>
                  </div>
                </div>
              `;
            }).join("")
        : `<div class="empty">Nenhum pedido para este cliente.</div>`;

      const suggestions = getSuggestions(clientId);

      const suggestionsHTML = suggestions.length
        ? suggestions.slice(0, 15).map(function(item) {
            const supplier = getSupplier(item.product.supplierId);

            return `
              <div class="list-item">
                <strong>${escapeHTML(item.product.name)}</strong>

                <div class="muted">
                  SKU: ${escapeHTML(item.product.sku)}
                  · ${abcBadge(item.curve)}
                  · ${escapeHTML(supplier?.name || "Sem fornecedor")}
                </div>
              </div>
            `;
          }).join("")
        : `<div class="empty">Nenhuma sugestão disponível.</div>`;

      const lowerHTML = getLowerPurchases(clientId).length
        ? getLowerPurchases(clientId).map(function(item) {
            return `
              <div class="list-item">
                <strong>${escapeHTML(item.product.name)}</strong>

                <div class="muted">
                  Comprado pelo cliente:
                  <strong>${item.clientQuantity}</strong>
                  · Média:
                  <strong>${item.average.toFixed(1)}</strong>
                </div>

                <div class="field" style="margin-top:8px">
                  <label>Motivo da compra menor</label>

                  <input
                    value="${escapeHTML(item.reason)}"
                    placeholder="Informe o motivo..."
                    onchange="saveLowerReason('${clientId}','${item.product.id}',this.value)">
                </div>
              </div>
            `;
          }).join("")
        : `<div class="empty">Nenhum produto abaixo da média.</div>`;

      document.getElementById("client-profile").innerHTML = `
        <div class="profile-header">
          <div>
            <button
              class="button small"
              onclick="showPage('clientes');renderAll()">
              ← Voltar
            </button>

            <h2 style="margin-top:14px">${escapeHTML(client.name)}</h2>

            <div class="muted">
              ${escapeHTML(client.phone || "Sem telefone")}
              · ${escapeHTML(client.email || "Sem e-mail")}
              · ${escapeHTML(client.city || "Sem cidade")}
            </div>
          </div>

          <div class="actions" style="margin-top:0">
            <button
              class="button primary"
              onclick="openSaleModal('${client.id}')">
              + Nova venda
            </button>

            <button
              class="button"
              onclick="document.getElementById('attachment-input').click()">
              Anexar arquivo
            </button>

            <input
              id="attachment-input"
              type="file"
              hidden
              onchange="saveAttachment('${client.id}', this.files[0])">
          </div>
        </div>

        <div class="cards">
          <div class="card">
            <div class="metric-label">Pedidos</div>
            <div class="metric-value">${stats.sales.length}</div>
          </div>

          <div class="card">
            <div class="metric-label">Itens comprados</div>
            <div class="metric-value">${stats.items}</div>
          </div>

          <div class="card">
            <div class="metric-label">Faturamento</div>
            <div class="metric-value green">${money(stats.revenue)}</div>
          </div>

          <div class="card">
            <div class="metric-label">Status</div>
            <div class="metric-value" style="font-size:16px">
              ${getClientStatus(client)}
            </div>
          </div>
        </div>

        <div class="profile-columns">
          <div>
            <div class="panel">
              <h2>Fornecedores do cliente</h2>

              <div class="chips">
                ${suppliersHTML}
              </div>

              <div class="muted" style="margin-top:10px">
                Colorido: já comprou deste fornecedor.
                Cinza: ainda não comprou.
              </div>
            </div>

            <div class="panel">
              <h2>Histórico de pedidos</h2>
              <div class="list">${ordersHTML}</div>
            </div>

            <div class="panel">
              <h2>Anexos</h2>
              ${renderAttachments(clientId)}
            </div>
          </div>

          <div>
            <div class="panel">
              <h2>Sugestões de produtos</h2>
              <div class="list">${suggestionsHTML}</div>
            </div>

            <div class="panel">
              <h2>Produtos abaixo da média</h2>
              <div class="list">${lowerHTML}</div>
            </div>
          </div>
        </div>
      `;

      showPage("profile");
    }

    function saveLowerReason(clientId, productId, reason) {
      const existing = database.lowerReasons.find(function(item) {
        return item.clientId === clientId &&
          item.productId === productId;
      });

      if (existing) {
        existing.reason = reason;
      } else {
        database.lowerReasons.push({
          id: createId("reason"),
          clientId: clientId,
          productId: productId,
          reason: reason
        });
      }

      saveDatabase();
    }

    function renderAttachments(clientId) {
      const files = database.attachments.filter(function(file) {
        return file.clientId === clientId;
      });

      if (!files.length) {
        return `<div class="empty">Nenhum anexo cadastrado.</div>`;
      }

      return `
        <div class="list">
          ${files.map(function(file) {
            return `
              <div class="list-item">
                <strong>${escapeHTML(file.name)}</strong>

                <div class="muted">
                  Adicionado em ${dateBR(file.date)}
                </div>

                <div class="actions">
                  <a
                    class="button small"
                    href="${file.data}"
                    download="${escapeHTML(file.name)}">
                    Baixar
                  </a>

                  <button
                    class="button small danger"
                    onclick="deleteAttachment('${file.id}','${clientId}')">
                    Excluir
                  </button>
                </div>
              </div>
            `;
          }).join("")}
        </div>
      `;
    }

    function saveAttachment(clientId, file) {
      if (!file) return;

      const reader = new FileReader();

      reader.onload = function() {
        database.attachments.push({
          id: createId("file"),
          clientId: clientId,
          name: file.name,
          type: file.type,
          data: reader.result,
          date: today()
        });

        saveDatabase();
        openClientProfile(clientId);
      };

      reader.readAsDataURL(file);
    }

    function deleteAttachment(fileId, clientId) {
      if (!confirm("Excluir este anexo?")) return;

      database.attachments = database.attachments.filter(function(file) {
        return file.id !== fileId;
      });

      saveDatabase();
      openClientProfile(clientId);
    }

    function getWarrantyPendencies() {
      const result = [];

      database.sales.forEach(function(sale) {
        (sale.items || []).forEach(function(item) {
          if (!item.warrantyActive) return;

          const product = getProduct(item.productId);
          const client = getClient(sale.clientId);

          if (product && client) {
            result.push({
              sale: sale,
              item: item,
              product: product,
              client: client
            });
          }
        });
      });

      return result;
    }

    function getSaleSuppliers(sale) {
      const suppliers = [];

      (sale.items || []).forEach(function(item) {
        const supplier = getSupplier(item.supplierId);

        if (supplier && !suppliers.includes(supplier.name)) {
          suppliers.push(supplier.name);
        }
      });

      return suppliers.map(escapeHTML).join(", ") || "—";
    }

    function openOrder(saleId) {
      const sale = database.sales.find(function(item) {
        return item.id === saleId;
      });

      if (!sale) return;

      const client = getClient(sale.clientId);

      const rows = sale.items.map(function(item) {
        const product = getProduct(item.productId);
        const supplier = getSupplier(item.supplierId);

        return `
          <tr>
            <td>
              <strong>${escapeHTML(product?.name || "Produto removido")}</strong>
              <br>
              <span class="muted">
                SKU: ${escapeHTML(item.sku || "—")}
              </span>
            </td>

            <td>${supplier ? supplierChip(supplier, true) : "—"}</td>
            <td>${item.quantity}</td>
            <td>${money(item.price)}</td>
            <td class="green">${money(item.quantity * item.price)}</td>

            <td>
              ${
                item.warrantyActive
                  ? `<span class="badge badge-active">Ativa</span>`
                  : `<span class="badge badge-inactive">Inativa</span>`
              }
            </td>

            <td>
              ${
                item.warrantyActive
                  ? ""
                  : `
                    <button
                      class="button small success"
                      onclick="activateWarranty('${sale.id}','${item.productId}')">
                      Ativar
                    </button>
                  `
              }
            </td>
          </tr>
        `;
      }).join("");

      document.getElementById("order-details").innerHTML = `
        <div class="card">
          <strong>${escapeHTML(client?.name || "Cliente removido")}</strong>

          <div class="muted">
            ${escapeHTML(client?.phone || "Sem telefone")}
            · ${escapeHTML(client?.email || "Sem e-mail")}
          </div>

          <div class="muted" style="margin-top:7px">
            Data: ${dateBR(sale.date)}
            · Vendedor: ${escapeHTML(getSeller(sale.sellerId)?.name || "—")}
            · Canal: ${escapeHTML(sale.channel || "—")}
          </div>
        </div>

        <div class="table-container" style="margin-top:15px">
          <table>
            <thead>
              <tr>
                <th>Produto</th>
                <th>Fornecedor</th>
                <th>Qtd.</th>
                <th>Preço</th>
                <th>Total</th>
                <th>Garantia</th>
                <th>Ação</th>
              </tr>
            </thead>
            <tbody>${rows}</tbody>
          </table>
        </div>

        <div style="margin-top:18px;text-align:right;font-size:20px">
          Total:
          <strong class="green">${money(getSaleTotal(sale))}</strong>
        </div>

        ${
          sale.notes
            ? `
              <div class="card" style="margin-top:15px">
                <strong>Observações</strong>
                <div class="muted" style="margin-top:6px">
                  ${escapeHTML(sale.notes)}
                </div>
              </div>
            `
            : ""
        }

        <div class="actions">
          <button
            class="button primary"
            onclick="downloadPDF('${sale.id}')">
            Baixar PDF
          </button>
        </div>
      `;

      document.getElementById("order-modal").classList.add("open");
    }

    function activateWarranty(saleId, productId) {
      const sale = database.sales.find(function(item) {
        return item.id === saleId;
      });

      if (!sale) return;

      const item = sale.items.find(function(item) {
        return item.productId === productId;
      });

      const product = getProduct(productId);

      if (!item || !product) return;

      const start = new Date();
      const end = new Date(start);

      end.setDate(end.getDate() + Number(product.warrantyDays || 0));

      item.warrantyActive = true;
      item.warrantyStart = start.toISOString().substring(0, 10);
      item.warrantyEnd = end.toISOString().substring(0, 10);

      saveDatabase();
      renderAll();
      openOrder(saleId);

      alert("Garantia ativada com sucesso.");
    }

    function downloadPDF(saleId) {
      const sale = database.sales.find(function(item) {
        return item.id === saleId;
      });

      if (!sale) return;

      const PDF = window.jspdf?.jsPDF;

      if (!PDF) {
        alert("Não foi possível carregar o gerador de PDF.");
        return;
      }

      const client = getClient(sale.clientId);
      const pdf = new PDF();

      let y = 20;

      pdf.setFillColor(229, 9, 20);
      pdf.rect(0, 0, 210, 10, "F");

      pdf.setTextColor(0, 0, 0);
      pdf.setFontSize(18);
      pdf.text("PEDIDO COMERCIAL", 15, y);

      y += 10;
      pdf.setFontSize(10);

      pdf.text("Cliente: " + (client?.name || "—"), 15, y);
      y += 6;

      pdf.text("Telefone: " + (client?.phone || "—"), 15, y);
      y += 6;

      pdf.text("Data: " + dateBR(sale.date), 15, y);
      y += 6;

      pdf.text(
        "Vendedor: " +
        (getSeller(sale.sellerId)?.name || "—") +
        " | Canal: " +
        (sale.channel || "—"),
        15,
        y
      );

      y += 12;

      pdf.setFillColor(40, 40, 40);
      pdf.setTextColor(255, 255, 255);
      pdf.rect(15, y - 5, 180, 8, "F");

      pdf.text("Produto / SKU", 18, y);
      pdf.text("Fornecedor", 95, y);
      pdf.text("Qtd.", 137, y);
      pdf.text("Total", 173, y);

      y += 9;
      pdf.setTextColor(0, 0, 0);
      pdf.setFontSize(9);

      sale.items.forEach(function(item) {
        const product = getProduct(item.productId);
        const supplier = getSupplier(item.supplierId);

        pdf.text(
          (
            product?.name || "Produto removido"
          ).substring(0, 35) +
          " / " +
          (item.sku || "—"),
          18,
          y
        );

        pdf.text(
          (supplier?.name || "—").substring(0, 20),
          95,
          y
        );

        pdf.text(String(item.quantity), 137, y);
        pdf.text(money(item.quantity * item.price), 173, y);

        y += 7;

        if (y > 270) {
          pdf.addPage();
          y = 20;
        }
      });

      y += 8;
      pdf.setFontSize(13);
      pdf.text("TOTAL: " + money(getSaleTotal(sale)), 145, y);

      if (sale.notes) {
        y += 12;
        pdf.setFontSize(10);
        pdf.text("Observações:", 15, y);
        y += 6;
        pdf.text(pdf.splitTextToSize(sale.notes, 175), 15, y);
      }

      pdf.save("pedido-" + (sale.date || today()) + ".pdf");
    }

    document.getElementById("finance-form").addEventListener("submit", function(event) {
      event.preventDefault();

      database.finances.push({
        id: createId("finance"),
        type: document.getElementById("finance-type").value,
        description: document.getElementById("finance-description").value.trim(),
        value: Number(document.getElementById("finance-value").value || 0),
        due: document.getElementById("finance-due").value,
        status: document.getElementById("finance-status").value,
        createdAt: today()
      });

      saveDatabase();
      event.target.reset();
      renderFinance();

      alert("Movimentação financeira salva.");
    });

    function renderFinance() {
      let receivable = 0;
      let payable = 0;
      let received = 0;

      database.finances.forEach(function(item) {
        if (item.type === "receber") {
          if (item.status === "pendente") {
            receivable += item.value;
          } else {
            received += item.value;
          }
        }

        if (item.type === "pagar" && item.status === "pendente") {
          payable += item.value;
        }
      });

      const result = received - payable;

      document.getElementById("finance-receivable").textContent =
        money(receivable);

      document.getElementById("finance-payable").textContent =
        money(payable);

      document.getElementById("finance-received").textContent =
        money(received);

      document.getElementById("finance-result").textContent =
        money(result);

      document.getElementById("finance-table").innerHTML =
        database.finances.length
          ? database.finances
              .slice()
              .reverse()
              .map(function(item) {
                return `
                  <tr>
                    <td>
                      <span class="badge ${
                        item.type === "receber"
                          ? "badge-active"
                          : "badge-inactive"
                      }">
                        ${
                          item.type === "receber"
                            ? "A receber"
                            : "A pagar"
                        }
                      </span>
                    </td>

                    <td>${escapeHTML(item.description)}</td>
                    <td>${money(item.value)}</td>
                    <td>${dateBR(item.due)}</td>
                    <td>${escapeHTML(item.status)}</td>

                    <td>
                      <button
                        class="button small danger"
                        onclick="deleteFinance('${item.id}')">
                        Excluir
                      </button>
                    </td>
                  </tr>
                `;
              }).join("")
          : `
            <tr>
              <td colspan="6" class="empty">
                Nenhuma movimentação financeira.
              </td>
            </tr>
          `;
    }

    function deleteFinance(financeId) {
      database.finances = database.finances.filter(function(item) {
        return item.id !== financeId;
      });

      saveDatabase();
      renderFinance();
    }

    function sendBirthday(clientId) {
      const client = getClient(clientId);

      if (!client || !client.phone) {
        alert("O cliente não possui telefone cadastrado.");
        return;
      }

      const phone = client.phone.replace(/\D/g, "");

      const message = encodeURIComponent(
        "Olá, " + client.name +
        "! Desejamos um feliz aniversário, muita saúde e sucesso!"
      );

      window.open(
        "https://wa.me/55" + phone + "?text=" + message,
        "_blank"
      );
    }

    function closeModal(id) {
      document.getElementById(id).classList.remove("open");
    }

    document.querySelectorAll(".modal").forEach(function(modal) {
      modal.addEventListener("click", function(event) {
        if (event.target === modal) {
          modal.classList.remove("open");
        }
      });
    });

    renderAll();
  </script>
</body>
</html>
