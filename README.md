# Ordem de Serviços – BambuLab

Sistema web para gerenciamento de ordens de serviço de manutenção e garantia de impressoras BambuLab.

## Como usar

### Criar uma nova OS

1. Clique em **+ Nova Ordem de Serviço** na barra lateral
2. Preencha os campos de **Identificação da OS** (nome e número do chamado)
3. Informe os **Dados do Cliente** (nome, CPF/CNPJ e endereço)
4. Preencha as **Informações da Máquina** (números de série e modelo)
5. Marque os **Itens Recebidos** junto com a máquina
6. Selecione o **Estado de Recebimento** (Bom estado ou Danificada)
7. Descreva o **Problema** relatado pelo cliente
8. Após o atendimento, preencha o **Serviço Realizado**
9. Informe as **Datas** e os **Técnicos Responsáveis**
10. Clique em **Salvar e Gerar PDF**

### Gerar PDF

O PDF é gerado automaticamente ao salvar a OS. Uma janela de impressão será aberta — basta salvar como PDF pelo navegador.

### Buscar e editar uma OS

- Use a barra de **busca** na lateral para filtrar por nome do cliente ou nome da OS
- Clique em qualquer OS da lista para carregar os dados no formulário
- Edite os campos e clique em **Salvar e Gerar PDF** novamente para atualizar

### Limpar o formulário

Clique em **Limpar tudo** para resetar todos os campos sem apagar as OS salvas.

## Modelos suportados

| Modelo    |
|-----------|
| A1 mini   |
| A1        |
| A2L       |
| P1        |
| P2        |
| X1        |
| X2        |
| H2        |
| AMS       |
| AMS 2     |
| AMS 2 Pro |

## Informações técnicas

- Os dados são salvos localmente no navegador via `localStorage`
- Não requer backend ou banco de dados
- Funciona em qualquer navegador moderno
- Responsivo para dispositivos móveis
