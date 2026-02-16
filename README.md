# CPF Válido

Ferramenta leve e reproduzível para validar matematicamente números de CPF diretamente no navegador.

Live website:  
https://helenopaiva.github.io/CPF/

---

## O que faz

Dado um CPF (com ou sem pontuação), o sistema:

Remove automaticamente caracteres não numéricos.
Verifica se o número possui 11 dígitos.
Invalida sequências repetidas (ex.: 11111111111).
Calcula o primeiro dígito verificador usando pesos de 10 a 2.
Calcula o segundo dígito verificador usando pesos de 11 a 2.
Compara os dígitos calculados com os informados.
Identifica a região fiscal a partir do 9º dígito.
Permite gerar CPFs matematicamente válidos para teste.
Permite copiar o número limpo ou mascarado.

A validação é exclusivamente matemática.

---

## Como usar a página

Acesse o site.
Insira ou cole um CPF.
O sistema valida automaticamente ao completar 11 dígitos.
Os detalhes do cálculo podem ser visualizados na seção expandível.

O projeto é um arquivo HTML único, executado integralmente no cliente.
Não há backend.
Não há requisições externas de dados.

---

## Arquitetura

Projeto estático com:

HTML5  
JavaScript Vanilla  
TailwindCSS via CDN  

Toda a lógica de validação é implementada em JavaScript no próprio arquivo `index.html`.

Não há armazenamento de dados.
Nenhuma informação é enviada para servidores.

---

## Limitações

Valida apenas a consistência matemática do CPF.

Não realiza:
Consulta à Receita Federal  
Verificação de situação cadastral  
Confirmação de existência do CPF  

Um CPF pode ser matematicamente válido e ainda assim estar cancelado ou inexistente.

---

## Autor

Desenvolvido e mantido por  
Heleno de Paiva Oliveira, MD, PhD  
Professor de Anestesiologia  
Universidade Federal do Rio Grande do Norte (UFRN)
