# 🧾 Gerador de Faturas (Invoice Generator)

<div align="center">

![Status](https://img.shields.io/badge/Status-Concluído-success)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

**Uma solução Single-Page, leve e pronta para impressão A4.**

[Funcionalidades](#-funcionalidades) • [Como Usar](#-como-usar) • [Estrutura](#-estrutura-do-código) • [Tecnologias](#-tecnologias)

</div>

---

## 📝 Sobre o Projeto

Este é um sistema simples e eficiente para geração de faturas de serviço. Desenvolvido com foco na **experiência do usuário (UX)** e na **qualidade de impressão**. O sistema funciona inteiramente no navegador, sem necessidade de servidores ou instalação de softwares complexos.

O diferencial é o uso inteligente de **CSS Media Queries**, permitindo que a tela de edição seja interativa, mas a impressão (ou PDF) saia limpa e profissional.

---

## ✨ Funcionalidades

* **⚡ Edição em Tempo Real:** A fatura é atualizada instantaneamente enquanto você digita.
* **🖨️ Otimizado para Impressão (A4):** Layout ajustado milimetricamente para folhas A4.
* **👁️ Preview Fiel:** O que você vê na tela é exatamente o que será impresso (`WYSIWYG`).
* **🌗 Interface Limpa:** Painel de controle fixo (`sticky`) para facilitar a edição de faturas longas.
* **📄 Exportação PDF:** Utiliza a função nativa do navegador para salvar como PDF vetorizado.
* **🎨 Formatação Automática:** Datas convertidas para PT-BR e valores monetários para BRL (R$) automaticamente.

---

## 🚀 Como Usar

Não é necessário instalar Node.js, Python ou servidores. É **Puro HTML/JS**.

1.  Baixe o arquivo `index.html`.
2.  Dê um duplo clique para abrir em seu navegador favorito (Chrome, Edge, Firefox, Brave).
3.  Preencha os campos no menu lateral esquerdo.
4.  Clique no botão **"🖨️ Imprimir / Salvar PDF"**.
5.  Na janela de impressão, selecione **"Salvar como PDF"** ou escolha sua impressora.

> **Dica:** Certifique-se de marcar a opção "Gráficos de plano de fundo" nas configurações de impressão do navegador para que as cores (cabeçalho, tabelas) saiam corretamente.

---

## 📂 Estrutura do Código

O projeto segue o conceito de **Single File Component** para fins didáticos:

```text
/
└── index.html  <-- Toda a mágica acontece aqui (HTML + CSS + JS)
```
Detalhes Técnicos
 * HTML Semântico: Uso de tags apropriadas (header, section, footer) para melhor acessibilidade.
 * CSS Variables: Cores definidas em :root para fácil customização de tema.
 * CSS Flexbox: Utilizado para o layout responsivo da interface de edição.
 * @media print: A "alma" do projeto. Define regras que ocultam o formulário e formatam a fatura apenas quando o comando de impressão é acionado.
 * Vanilla JavaScript: Lógica leve sem dependências (sem jQuery, React ou Vue) para máxima performance.
🎨 Personalização
Quer colocar a cor da sua empresa? Abra o arquivo fatura.html em um editor de texto e procure por:
:root {
    --primary-color: #2c3e50; /* Mude aqui a cor principal */
    --accent-color: #3498db;  /* Mude a cor de destaque */
}

Para alterar o logo/nome da empresa, edite a linha 297 no HTML:
<div class="company-name">SUA EMPRESA AQUI</div>

🤝 Contribuição
Sinta-se livre para clonar e melhorar este projeto! Ideias para evoluir:
 * [ ] Adicionar suporte a múltiplos itens na tabela.
 * [ ] Cálculo automático de impostos (ISS/ICMS).
 * [ ] Upload de Logotipo (imagem).
 * [ ] Opção para salvar histórico no localStorage.
<div align="center">
Feito com 💙.
</div>
