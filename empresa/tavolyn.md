# Tavolyn

Empresa de sistemas comerciais. Sócios: **Stefano Moretti** e **Leonardo Culler**.

## Produto: PDV para restaurantes

Sistema de ponto de venda em Node.js + MySQL, com interface em HTML/CSS/JS puros. Código em `C:\Users\Stefano Moretti\Desktop\pdv-restaurante` (GitHub `stefanomrtt/pdv-restaurante`).

| Módulo | Resumo |
|---|---|
| Salão | Mapa de mesas, comanda, taxa de serviço, divisão, transferência |
| Balcão | Venda rápida sem mesa |
| Delivery | Quadro por status, taxa de entrega, roteirização e mapa dos motoboys |
| Cozinha (KDS) | Produção em tempo real, com cronômetro e alerta de atraso |
| Caixa | Abertura, sangria, suprimento, conferência e fechamento |
| Estoque | Insumos, ficha técnica, baixa automática, perdas, inventário |
| Clientes | Cadastro pelo telefone, endereços, histórico |
| WhatsApp | Robô com IA (Claude Haiku) monta o pedido; a equipe confere |
| Integrações | Webhook para bots de WhatsApp e apps de delivery (iFood, Rappi) |
| Relatórios e Inteligência | Faturamento, curva ABC, picos, clima, clientes para reconquistar |
| Gemini Notebook | Perguntas sobre o histórico, com fontes no Google Drive |
| App do motoboy | PWA com rota, navegação por voz e "entreguei" com GPS |

## Plataforma

- Cada restaurante tem banco e endereço próprios: `<loja>.tavolyn.com.br`.
- `painel.tavolyn.com.br`: painel dos sócios (clientes, contratos, MRR, funil, saúde do servidor, auditoria).
- `tavolyn.com.br`: site da empresa.
- Servidor: AWS Lightsail em São Paulo; DNS no Registro.br (um registro A por restaurante, sem curinga).
- Lojas com impressora térmica usam o **agente de impressão** instalado no computador da loja.

## Clientes

Ver `empresa/clientes.md`.
