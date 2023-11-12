# Gerador de pdf para orçamentos em python.

Em dias atuais é extremamente comum o envio de orçamentos para nossos clientes.
Este simples modelo é funcional e bem prático. 

-------------------------------------------------------
### Com algumas linhas de código: 

```
from fpdf import FPDF

pdf = FPDF()
pdf.add_page()
pdf.set_font("Arial")

pdf.image("template.png", x=0, y=0)

projeto = input('Digite a descrição do projeto: ')
horas_estimadas = input('Digite o total de horas estimadas: ')
valor_hora = input('Digite o valor da hora trabalhada: ')
prazo_estimado = input('Digite o prazo estimado: ')

valor_total_estimado = int(horas_estimadas) * int(valor_hora)

pdf.text(115,145, projeto)
pdf.text(115,160, horas_estimadas)
pdf.text(115,175, valor_hora)
pdf.text(115,190, prazo_estimado)
pdf.text(115,205, str(valor_total_estimado))

pdf.output("orcamento.pdf")
print("Orçamento gerado com sucesso!")
```

### Podemos obter um pdf desses com velocidade.

![image](https://github.com/Henrique-de-Souza/Gerador_de_PDF/assets/148600312/365eab94-1653-4ea1-8747-96a6dd693f1b)

-----------------------------------------------------------------------------

Entre em contato:

email: empresa.henrique@outlook.com

telefone: (14) 9 9626-2918

instagram: @enriquedesu

-------------------------------------------------------------------------


