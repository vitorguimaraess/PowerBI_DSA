# Cap 3 - Modelagem de dados e relacionamento  

### **Modelagem de dados**: tecnícas para criar um blueprint.

Consiste em criar uma representação visual ou schema que define os sistemas de coleta ou gerenciamento de informacoes.
essa modelagem auxilia toda equipe de análise para criar relatórios, e entao criamos um modelo de dados para verificar como eles se relacionam. Buscamos os dados nas fontes, colocamos em um sistema de armazenamento e analise.
O modelo serve para descrever quais dados a empresa coleta, a relação entre os conjuntos e os metodos de armazenamento e análise.

Em resumo a modelagem serve para criar um **modelo conceitual, fisico ou logico** de dados.
#### Conceitual: conceitos e relações entre os dados.
#### Lógico: como os dados sao armazenados e como as relacoes sao representadas em um banco.</p>
#### Fisico: Descreve como os dados sao armazenados em um sistema de armazenameto especifico.</p>

O PBI simplifica de forma significativa esse processo criando um modelo de dados básico, mais eficiênte e que pode ser usado para analisar os dados de forma correta.

O PBI tambêm evita que erros de relacionamento ocorram se os dados não estiverem organizados corretamente.

PBI não criará os relacionamentos entre os dados se os dados não estiverem corretamente conectados. Porém permite criar gráficos e dashboards assim mesmo.

### Business Intelligence

Combina análise de negócios, mineração de dados, visualização de dados, ferramentas/infraestrutura de dados e práticas recomendadas para ajuda nas oraganizações para tomar decisões impulsinadas por dados.

Analisar o passado comprrendendo métricas e indicadores, padrões e relacionamanetos. O objetivo maior é a análise descritiva do que aconteceu.

Faz parte do universo da CD (Ciência de dados), mas CD tem foco maior em análise preditiva, olhando o futuro. "Sera que a campanha de marketing vai trazer mais clientes no proximo ano"

#### **Como aplicamos a modelagem de dados**

**Criação de um DW:** É um repositório centralizado de dados para análise e tomada de negócios que é usado para suportar a análise e tomada de decisão.

**Design de Cubos Multidimensionais:** A modelagem de dados é usada para projetar cubos multidimensionais, que são estruturas de dados que ajudam a agragar e analisar dados de várias fontes.

**Criação de um star schema:** Técinica comumente usada para projetar DWs, que ajuda a garantir a consistência e a facilidade de acesso aos dados.

**Otimização:** A modelagem tambem é usada para otimizar as consultas a um DW, garantindo que as consultas sejam executadas de forma eficiente.

**Integração de Dados:** A modelagem de dados é usada para integrar dados de várias fontes, garantido a consistencia dos dados.

**Governança de dados:** A modelagem de dados é importante para garantir a Qualidade dos dados e para implementar medidas de governança de dados como rastreamento de alterações e auditoria.


#### **Beneficios da modelagem de dados**

O PBI tem 3 paineis.
* Relatórios;
* Dados;
* Modelagem de dados.

Parte do trabalho de modelagem o PBI tenta fazer de forma automática. Tentando detectar o modelo certo.Se ele conseguir ele cria o modelo.
Se houver algum problema ele não consegue, você tem que checar, corrigir e então criar o modelo.

#### **Razões desses problemas**

**Importação de dados:** PBI permite importar dados de uma variedade de fontes, como BD's, Nuvens e Arquivos. A modelagem de dados é usada para preparar os dados importados, garantindo que eles estejam em um formato consistente e estruturado para análise.

**Tabelas e relações:** A modelagem é usada para criar tabelas e estabelecer relações entre elas, garantindo que os dados estejam organizados de forma lógica e coerente.

**Medidas e cálculos:** O Power BI permite criar medidas e cálculos personalizados como somas, médias e percentuais. A modelagem de dados é usada para garantir que esses cálculos sejam aplicados de forma consistente e correta.

**Filtros e Segmentação:** A modelagem de dados é usada para criar filtros e segmentações para os relatórios, permitindo que os usuários explorem os dados de forma mais precisa e detalhada.

**Publicação de relatórios e dash:** PBI permite publicação de relatórios e dashboards baseados na modelagem de dados, para que os usuários possam acessá-los e explorá-los facilmente.

Sempre verifique o modelo de dados no PBI quando estiver usando mais de uma fonte de dados.

Compreenda o que são os relacionamentos de negócio.

**Por exemplo:** *Cada produto pode estar associado a mais de uma venda*
Assim estabeleça o relacionamento no PBI (ele tentará fazer isso de forma automática)

Observe os relacionamentos entre os dados e considere desmembrar uma única planilha ou tabela em diferentes partes para construir o relacionamento adequado. (Planilha com 50, 100 colunas, que vieram de várias), considere quebra-lá de volta em várias.

Faça ajustes e correções nos dados para estabelecer os relacionamentos.
### Forma de realizar ajustes:
verificando a incidência de ID's
1. Passo Agrupe a coluna e traga uma contagem de quantas vezes aquela linha aparece na coluna
![Passo1VerificandoQTDdeIDporRelacionamento](https://github.com/vitorguimaraess/PowerBI_DSA/assets/110196971/c9d441a6-eb44-4d22-8d69-f6f40f625dea)
![Passo2 Agrupe, para contar a qtd de vezs q esses IDs aparecem](https://github.com/vitorguimaraess/PowerBI_DSA/assets/110196971/4bb170e0-de1c-4562-968a-ce53794ed05f)

### *Cardinalidades*
https://go.microsoft.com/fwlink/?linkid=2011502

<table>
  <tr>
    <td>1 para muitos</td>
    <td>1 para 1</td>
    <td>1 para muitos</td>
  </tr>
  <tr>
    <td>(1,*)</td>
    <td>(1,1)</td>
    <td>(*,*)</td>
  </tr>
</table>
