# Dividi — protótipo funcional

Aplicativo front-end responsivo para dividir despesas em grupo.

## Como executar
1. Extraia o ZIP para uma pasta.
2. Abra `index.html` no navegador, ou abra a pasta no VS Code e use a extensão Live Server.
3. Os dados de demonstração e suas alterações ficam salvos no `localStorage` deste navegador.

## O que funciona
- Painel responsivo, grupos e participantes sem necessidade de conta.
- Criação de grupo com moeda padrão.
- Registro de despesa com divisão igualitária, valores exatos, percentagens ou quotas.
- Validação dos valores e arredondamento em centavos.
- Conversão de moeda usando a API pública Frankfurter (`api.frankfurter.app`), sem chave de API.
- Saldo líquido e sugestões de acerto de contas.
- Registro de pagamentos parciais e totais.
- Filtros por categoria, participante, texto e data.
- Histórico local de pagamentos e despesas.

## Limitações importantes
- Este é um protótipo front-end. Não tem autenticação real, sincronização entre dispositivos, convites, banco de dados na nuvem ou proteção multiusuário.
- A taxa de câmbio depende da disponibilidade da API. Se não houver taxa disponível, o app não inventa uma nem salva a despesa.
- A API Frankfurter usa taxas de referência e não é uma cotação comercial garantida para transferências.
- Os membros sem conta são registros locais, não convites enviados a pessoas reais.
- Para produção, adicione backend/API, autenticação, banco de dados, autorização por grupo, trilha de auditoria, testes e políticas de privacidade.

## Arquivos
- `index.html`: estrutura da interface.
- `styles.css`: layout responsivo e estilos.
- `app.js`: estado, cálculos, validação, câmbio e renderização.
