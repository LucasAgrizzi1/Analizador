# Analizador
Utiliza Azure AI Document Intelligence (Inteligência de Documentos) e Azure AI Vision (Visão)
Logica em 3 etapas
  1.Extração de Dados e Score de Confiança (Document Intelligence)
  2.Verificação de Consistência e Validade (Lógica de Negócio)
  3.Correspondência de Identidade (Azure AI Vision):

Como Funciona:

O código usa o modelo prebuilt-idDocument para extrair campos como nome, número do documento e data de nascimento.
Para cada campo, o Azure retorna um confidence score (confiança).
pós a extração, você aplica regras de negócio.
Usa o Azure AI Face para comparar a foto do documento com a selfie e determinar a probabilidade de serem a mesma pessoa.

