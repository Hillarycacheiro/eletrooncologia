# Eletrooncologia — Sistema Frontend

React + Vite + Bootstrap com Dark/Light Mode e tela de login.

## 🚀 Instalação

```bash
npm install
npm run dev
# → http://localhost:5173
```

## 🔑 Login de teste

- **E-mail:** admin@eletrooncologia.com
- **Senha:** onco123

## 🔌 API C# — CORS (Program.cs)

```csharp
builder.Services.AddCors(options =>
    options.AddPolicy("Frontend", p =>
        p.WithOrigins("http://localhost:5173")
         .AllowAnyHeader().AllowAnyMethod()));

app.UseCors("Frontend");
```

## 📁 Estrutura

```
src/
├── components/   Field, Modal, SaveToast, Sidebar, Topbar
├── pages/        LoginPage, Dashboard, Empresa, Produto, Aplicacao, Cliente, Parceria
├── services/     api.js (Axios + todos os endpoints)
├── styles/       global.css (tokens dark + light)
├── App.jsx       Rotas + auth guard + theme state
└── main.jsx      Entry point
```
