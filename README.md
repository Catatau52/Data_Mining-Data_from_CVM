# Data_Mining-Data_from_CVM

Mineração de dados dos balanços que as empresas de capital aberto reportam à CVM.

O código tem como objetivo:
 - Capturar os balanços dos seguintes documentos das empresas de capital aberto de 2011 até 2022.
     - Balanço Patrimonial Ativo (BPA)
     - Balanço Patrimonial Passivo (BPP)
     - Demonstração de Resultado (DRE)
     - Demonstração de Valor Adicionado (DVA)
 - Filtrar os principais balanços dos documentos.
     - A escala da moeda de todos os resultados está em 'MIL', ou seja, basta multiplicar alguns valores por 1000.
 - Criar um novo data frame com indicadores fundamentalistas a partir dos resultados dos balanços que sejam idenpendentes do preço (preço da lib Yahoo finance contem erros :/ )
 - Legenda. (Os indicaores foram retirados de diversas fontes públicas na internet, para serem aplicadas em um modelo matemático no futuro.)
     - VPA = Valor Patrimonial por Ação
     - LPA_BASE = Lucro por Ação fornecido no balanço
     - LPA_CALC = Lucro por Ação Calculado atráves do (Lucro / Númeroe de ações)
     - PAYOUT = Distribuição de lucros aos acionistas (Dividendos + Juros por Capital próprio)
     - PL/ATIVOS = Patrimônio Líquido / Ativos
     - PASSIVOS/ ATIVOS = 
     - DIV/PL = Dívida Líquida / Patrimônio Líquido : (Dívida Líquida = Passivos Circulantes - Caixa)
     - DIV/EBIT = Dívida Líquida / EBIT : (Dívida Líquida = Passivos Circulantes - Caixa)
     - DIV/EBITDA = Dívida Líquida / EBITDA : (Dívida Líquida = Passivos Circulantes - Caixa)
     - M.EBITDA = EBITDA / Receita
     - ROE = Lucro / Patrimônio Líquido
     - ROIC = EBIT/ (Patrimônio Líquido + Dívida Longa) : (Dívida Longa = Passivo Total - Passivos Circulantes )
     - ROA = Lucro / Ativos
     - ILC = Ativo Circulante / Passivo Circulante
     - MLB = Lucro Bruto / Receita
     - MLO = EBIT / Receita
     - MLL = Lucro / Receita
     - VLE = Variação do lucro trimestral.
     - Ações_ON = Número de ações ordinárias
     - Ações_PN = Número de ações preferências 
     - Tes_ON = Número de ações ordinárias em tesouraria
     - Tes_ON = Número de ações preferências em tesouraria
     - FREE_FLOAT = Número de ações disponíveis - o Número de ações em tesouraria (Falta identificar os controladores relevantes)
     - TOTAL_ACOES = Número total de ações 
   
