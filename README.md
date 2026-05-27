# Fatec - Mineração de Dados

Breve projeto de Mineração de Dados para análise macroeconômica ("efeito tesoura").

Resumo para visitantes
- Objetivo: analisar a relação entre `Pagamento_Total_Divida` e `Gasto_Social` (saúde + educação) usando dados do World Bank (2010–2023).
- Principais técnicas: pré-processamento com `pandas`, clusterização com `KMeans` e mineração de regras com `Apriori` (`mlxtend`).
- Resultado principal: evidências de que cargas de dívida maiores tendem a pressionar gastos sociais.

Arquivos úteis
- Relatório (PDF): [Relatorio final Mineração.pdf](Relatorio final Mineração.pdf)
- Texto extraído do relatório: [Relatorio final Mineração.txt](Relatorio final Mineração.txt)
- Script de extração de PDF: [extract_pdf.py](extract_pdf.py)
- Notebooks principais: `13 anos enxugando gelo.ipynb` (análise) e `gráfco de 30 anos .ipynb` (anexado/uso histórico).

Rápido para rodar localmente
1. Ative o ambiente virtual (PowerShell):

```powershell
& .venv\Scripts\Activate.ps1
```

2. Instale dependências mínimas (se não existir `requirements.txt`):

```powershell
.venv\Scripts\python -m pip install PyPDF2 pandas scikit-learn mlxtend
```

3. Extrair o texto do relatório (gera `Relatorio final Mineração.txt`):

```powershell
.venv\Scripts\python extract_pdf.py "Relatorio final Mineração.pdf"
```

Observações rápidas
- O projeto usa os CSVs do World Bank já presentes no repositório.
- Para reproduzir a análise principal, abra `13 anos enxugando gelo.ipynb` no Jupyter/VS Code.

Contato
- Autor(es) no relatório: Luís Henrique da Silva, Pedro A. Batista, Tarsis Mikael Ventura Dumas de Lima.
