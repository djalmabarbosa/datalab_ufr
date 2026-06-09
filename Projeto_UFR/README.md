# Projeto UFR - submissao PROPGP

Este diretorio organiza a versao do projeto preparada para submissao ao Edital de Fluxo Continuo nº 001/PROPGP/UFR/2026.

## Versao recomendada para submissao

- Fonte editavel principal: `Projeto_UFR/8_projeto_pesquisa_v15_UFR_PROPGP.qmd`
- PDF renderizado: `Projeto_UFR/8_projeto_pesquisa_v15_UFR_PROPGP.pdf`
- DOCX editavel: `Projeto_UFR/8_projeto_pesquisa_v15_UFR_PROPGP.docx`
- Declaracao de projeto nao financiado: `Projeto_UFR/declaracao_projeto_nao_financiado_v15_UFR_PROPGP.docx` ou `Projeto_UFR/declaracao_projeto_nao_financiado_v15_UFR_PROPGP.pdf`

## Origem das versoes

- `CEP_resposta_pendencia_8477643/8_projeto_pesquisa_v14_pos_parecer.qmd`: versao pos-parecer preparada para resposta ao CEP, com ajustes eticos, LGPD, dados secundarios, TCLE e instrumentos anexos.
- `Projeto_UFR/8_projeto_pesquisa_v15_UFR_PROPGP.qmd`: versao derivada da v14 e ajustada para conferencia da PROPGP/UFR.

## Ajustes feitos na v15

- A fonte `8_projeto_pesquisa_v15_UFR_PROPGP.qmd` foi mantida textualmente igual a `CEP_resposta_pendencia_8477643/8_projeto_pesquisa_v14_pos_parecer.qmd`.
- Os ajustes para a PROPGP foram organizados fora do corpo do projeto, por meio deste README, da declaracao de projeto nao financiado e da reuniao dos arquivos de apoio na pasta `Projeto_UFR`.
- Foi copiado para esta pasta o arquivo `cronograma_execucao_v14.png`, mantendo a referencia original usada pela v14 e permitindo a renderizacao da v15.

## Arquivos de apoio

- `Projeto_UFR/Edital_de_Fluxo_Contínuo_001PROPGP-2026.pdf`: edital usado para conferencia.
- `Projeto_UFR/referencias_dashboards_extensao.bib`: base bibliografica usada pelo Quarto.
- `Projeto_UFR/custom_pesquisa.css`: folha de estilo para eventual renderizacao HTML.

## Checklist antes de submeter no SUAP

- Conferir se o cadastro no SUAP tem apenas uma meta para os 12 meses, com atividades internas.
- Assinar e anexar a declaracao de projeto nao financiado, pois o projeto nao possui financiamento externo especifico.
- Confirmar se a PROPGP exige algum documento adicional da Instrucao Normativa PROPGP/UFR nº 13/2025 alem dos anexos do edital.
- Conferir se o coordenador esta sem pendencias na PROPGP.
- Conferir se o grupo/nucleo de pesquisa esta certificado e atualizado no DGP/CNPq.
- Conferir se o Lattes dos docentes da equipe foi atualizado nos ultimos seis meses.
- Conferir no SUAP a inclusao do discente de graduacao da UFR.
- Conferir manualmente a apresentacao das referencias conforme exigencia ABNT do edital.
- Para o CEP, manter separado o pacote da pasta `CEP_resposta_pendencia_8477643`, pois ele atende a outra finalidade administrativa.

## Como renderizar novamente

No PowerShell, a partir desta pasta:

```powershell
& 'C:\Program Files\Positron\resources\app\quarto\bin\quarto.exe' render '8_projeto_pesquisa_v15_UFR_PROPGP.qmd' --to pdf
& 'C:\Program Files\Positron\resources\app\quarto\bin\quarto.exe' render '8_projeto_pesquisa_v15_UFR_PROPGP.qmd' --to docx
& 'C:\Program Files\Positron\resources\app\quarto\bin\quarto.exe' render 'declaracao_projeto_nao_financiado_v15_UFR_PROPGP.qmd' --to docx
```
