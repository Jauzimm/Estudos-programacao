# Escolha do Processo de Desenvolvimento de Software

Para selecionar um processo de desenvolvimento, é necessário responder a questões técnicas, humanas e organizacionais relacionadas ao sistema, ao time de desenvolvimento e à organização envolvida. **Não é uma receita de bolo**; o engenheiro de software deve conhecer os modelos e o contexto do produto para tomar decisões adequadas.

## Critérios Propostos por Sommerville (2018)

Sommerville sugere avaliar três tipos de questões para equilibrar abordagens dirigidas por plano ou ágil:

### Questões Técnicas (Sistema)
1. Qual é o tamanho do sistema a ser desenvolvido?
2. Que tipo de sistema está sendo desenvolvido?
3. Qual é a vida útil prevista para o sistema?
4. O sistema está sujeito a controle externo?

### Questões Humanas (Time)
1. Qual é o nível de competência dos projetistas e programadores?
2. Como está organizado o time de desenvolvimento?
3. Quais tecnologias estão disponíveis para apoiar o desenvolvimento?

### Questões Organizacionais (Organização)
1. É importante ter uma especificação detalhada antes da implementação?
2. É viável uma estratégia de entrega incremental?
3. Os representantes do cliente estarão disponíveis para colaborar?
4. Existem questões culturais que possam influenciar o desenvolvimento?

---

## Modelos de Ciclo de Vida

### Modelo Cascata
- Processo linear com etapas únicas.
- Adequado para projetos com requisitos bem definidos.

### Modelo Incremental
- Semelhante ao cascata, mas com entregas antecipadas.
- Ideal para requisitos conhecidos, mas possivelmente instáveis.

### Modelo Evolutivo
- Requisitos revisados em cada ciclo.
- Útil quando os requisitos não estão totalmente definidos.

### Modelo Espiral
- Foco no controle de riscos.
- Requer gerenciamento e habilidades de análise de riscos.

---

## Seleção de Modelo com Base em Características

### Requisitos
- A natureza e estabilidade dos requisitos são fundamentais na escolha do modelo.

| **Critério**                             | **Waterfall** | **Prototype** | **Iterative** | **Evolutionary** | **Spiral** | **RAD** |
|------------------------------------------|---------------|---------------|---------------|-------------------|------------|---------|
| Enhancements de sistemas existentes      | Não           | Não           | Sim           | Sim               | Não        | Sim     |
| Estabilidade do financiamento            | Sim           | Sim           | Não           | Não               | Não        | Sim     |
| Altos requisitos de confiabilidade       | Não           | Não           | Sim           | Sim               | Sim        | Não     |
| Prazos apertados                         | Não           | Sim           | Sim           | Sim               | Sim        | Sim     |
| Uso de componentes reutilizáveis         | Não           | Sim           | Não           | Não               | Sim        | Sim     |
| Recursos escassos                        | Não           | Sim           | Não           | Não               | Sim        | Não     |

### Status da Equipe
- Disponibilidade, competência e trabalho em equipe influenciam o modelo apropriado.

|| **Equipe de Desenvolvimento**                      | **Cascata** | **Protótipo** | **Melhoria Iterativa** | **Desenvolvimento Evolutivo** | **Espiral** | **RAD** |
|----------------------------------------------------|-------------|---------------|-------------------------|-------------------------------|-------------|---------|
| Pouca experiência em projetos similares            | Não         | Sim           | Não                     | Não                           | Sim         | Não     |
| Pouco conhecimento do domínio (nova tecnologia)    | Sim         | Não           | Sim                     | Sim                           | Sim         | Não     |
| Pouca experiência nas ferramentas a serem usadas   | Sim         | Não           | Não                     | Não                           | Sim         | Não     |
| Disponibilidade de treinamento, se necessário      | Não         | Não           | Sim                     | Sim                           | Não         | Sim     |


### Envolvimento do Usuário
- Maior participação do usuário favorece modelos mais iterativos e ágeis.

| **Critério**                              | **Waterfall** | **Prototype** | **Iterative** | **Evolutionary** | **Spiral** | **RAD** |
|-------------------------------------------|---------------|---------------|---------------|-------------------|------------|---------|
| Envolvimento do usuário em todas as fases | Não           | Sim           | Não           | Não               | Não        | Sim     |
| Participação limitada do usuário          | Sim           | Não           | Sim           | Sim               | Sim        | Não     |
| Usuários sem experiência anterior         | Não           | Sim           | Sim           | Sim               | Sim        | Não     |
| Usuários especialistas no domínio         | Não           | Sim           | Sim           | Não               | Não        | Sim     |

### Tipo de Projeto e Riscos
- Modelos como o espiral são melhores para projetos de alto risco.

| **Critério**                               | **Waterfall** | **Prototype** | **Iterative Enhancement** | **Evolutionary Development** | **Spiral** | **RAD** |
|--------------------------------------------|---------------|---------------|----------------------------|------------------------------|------------|---------|
| Projeto é a melhoria de um sistema existente | Não           | Não           | Sim                        | Sim                          | Não        | Sim     |
| Financiamento estável para o projeto        | Sim           | Sim           | Não                        | Não                          | Não        | Sim     |
| Altos requisitos de confiabilidade          | Não           | Não           | Sim                        | Sim                          | Sim        | Não     |
| Prazos apertados                            | Não           | Sim           | Sim                        | Sim                          | Sim        | Sim     |
| Uso de componentes reutilizáveis            | Não           | Sim           | Não                        | Não                          | Sim        | Sim     |
| Recursos (tempo, dinheiro, equipe etc.) escassos | Não           | Sim           | Não                        | Não                          | Sim        | Não     |

## Fatores que Influenciam a Escolha

### Sistema
- Tipo, vida útil, escala, regulação.

### Time
- Competência, tecnologia, distribuição.

### Organização
- Contratos, entrega, cultura.

