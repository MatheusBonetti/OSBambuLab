# Ordem de Serviços – BambuLab

Sistema web para gerenciamento de ordens de serviço de manutenção e garantia de impressoras BambuLab.

## Deploy no Vercel

### 1. Fork ou clone o repositório

Clique em **Fork** no canto superior direito desta página para copiar o repositório para sua conta do GitHub.

### 2. Acesse o Vercel

Entre em [vercel.com](https://vercel.com) e faça login com sua conta GitHub.

### 3. Importe o projeto

1. Clique em **Add New... → Project**
2. Na lista de repositórios, localize **OSBambuLab** e clique em **Import**

### 4. Configure o projeto

Nenhuma configuração adicional é necessária. O Vercel detecta automaticamente o `vercel.json` e faz o deploy como site estático.

Clique em **Deploy**.

### 5. Acesse o sistema

Após o deploy (leva cerca de 30 segundos), o Vercel fornece uma URL pública no formato:

```
https://os-bambulab.vercel.app
```

Pronto! A partir daí, qualquer atualização enviada ao repositório (git push) será publicada automaticamente.

---

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
