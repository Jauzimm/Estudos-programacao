# API

## O que é uma API?

API significa **Application Programming Interface** (Interface de Programação de Aplicação). APIs são mecanismos que permitem que dois componentes de software se comuniquem usando um conjunto de definições e protocolos. Em poucas palavras, APIs servem para conectar aplicativos.

Por exemplo: o sistema de software do instituto meteorológico contém dados meteorológicos diários. A aplicação para a previsão do tempo em seu telefone “fala” com esse sistema por meio de APIs e mostra atualizações meteorológicas diárias no telefone.

## Quais são os diferentes tipos de API?

As APIs são classificadas de acordo com sua arquitetura e escopo de uso:

### APIs privadas
- Internas a uma empresa.
- Usadas apenas para conectar sistemas e dados dentro da empresa.

### APIs públicas
- Abertas ao público, podendo ou não exigir autorização ou custos associados.

### APIs de parceiros
- Acessíveis apenas por desenvolvedores externos autorizados, auxiliando parcerias entre empresas.

### APIs compostas
- Combinam duas ou mais APIs distintas para atender a requisitos ou comportamentos complexos do sistema.

## Como as APIs funcionam?

A arquitetura da API geralmente é explicada em termos de cliente e servidor. A aplicação que envia a solicitação é chamada de cliente e a aplicação que envia a resposta é chamada de servidor. 

No exemplo do clima, o banco de dados meteorológico do instituto é o servidor e o aplicativo móvel é o cliente. 

### O que é um endpoint de API e por que ele é importante?
Os endpoints da API são os pontos de contato finais no sistema de comunicação, incluindo URLs de servidores e serviços. Eles são importantes por dois motivos:

1. **Segurança**: Vulneráveis a ataques, demandam monitoramento para impedir o uso indevido.
2. **Performance**: Endpoints de alto tráfego podem causar gargalos e afetar a performance do sistema.

### Maneiras de funcionamento das APIs

1. **APIs SOAP**
   - Usam o Simple Object Access Protocol.
   - Mensagens em XML.
   - Menos flexível, mais popular no passado.

2. **APIs RPC**
   - Remote Procedure Calls.
   - O cliente executa funções no servidor e recebe a saída.

3. **APIs WebSocket**
   - Comunicação bidirecional usando objetos JSON.
   - Mais eficientes que REST em alguns casos.

4. **APIs REST**
   - Transferência Representacional de Estado.
   - Operam via HTTP com funções como GET, PUT e DELETE.
   - Característica principal: ausência de estado.

## O que são APIs REST?

APIs REST permitem a troca de dados via HTTP. Suas principais características são:
- **Integração**: Aproveitamento de código existente.
- **Inovação**: Alterações no nível da API sem reescrita completa.
- **Expansão**: Atendem clientes em diferentes plataformas.
- **Facilidade de manutenção**: Alterações internas não afetam outras partes.

### Como proteger uma API REST?

1. **Tokens de autenticação**
   - Autorizam usuários e verificam direitos de acesso.

2. **Chaves de API**
   - Identificam aplicações e permitem monitoramento.

## O que é API Web?

Uma **API Web** é uma interface entre um servidor e um navegador. As APIs REST são um tipo especial de API Web, permitindo integração e automação de dados.

## O que são integrações de API?

Integrações de API são componentes que atualizam dados automaticamente entre clientes e servidores, como:
- Sincronização de dados na nuvem.
- Atualização automática de fuso horário.

## Como usar uma API?

1. Obtenha uma chave de API criando uma conta no provedor.
2. Configure um cliente de API HTTP.
3. Consulte a documentação para estruturar solicitações.
4. Implemente a API no código.

## Onde posso encontrar novas APIs?

Plataformas para encontrar APIs incluem:

- **RapidAPI**: Maior mercado global, com mais de 10.000 APIs públicas.
- **Public APIs**: Organiza APIs em 40 categorias.
- **APIForThat** e **APIList**: Listam mais de 500 APIs com detalhes sobre uso.

## REFERÊNCIA

- [https://aws.amazon.com/pt/what-is/api/](https://aws.amazon.com/pt/what-is/api/)
- [https://www.redhat.com/pt-br/topics/api/what-are-application-programming-interfaces](https://www.redhat.com/pt-br/topics/api/what-are-application-programming-interfaces)
- [https://www.youtube.com/watch?v=ByGJQzlzxQg](https://www.youtube.com/watch?v=ByGJQzlzxQg)
- [https://www.youtube.com/watch?v=bxuYDT-BWaI](https://www.youtube.com/watch?v=bxuYDT-BWaI)
- 