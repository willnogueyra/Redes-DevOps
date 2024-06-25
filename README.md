# Redes-DevOps
![Bpf-fundamentosroteamento-2.png](https://wiki.brasilpeeringforum.org/images/4/4c/Bpf-fundamentosroteamento-2.png)

> **OBS**: As quatro camadas do TCP/IP são: **de aplicação, de transporte, de rede (ou Internet) e de interface (ou enlace de dados)**
> 

# Camada de Aplicação

A camada de aplicação do modelo TCP/IP é a camada responsável por fornecer serviços de rede diretamente para as aplicações dos usuários finais. Nesta camada, os protocolos definem como as aplicações se comunicam através da rede, estabelecendo normas para a troca de dados e informações.

Um dos protocolos mais importantes e amplamente utilizados na camada de aplicação é o HTTP (HyperText Transfer Protocol). O HTTP é o protocolo subjacente da World Wide Web e permite a transferência de hipertextos, como páginas HTML, imagens, vídeos, entre outros.

Aqui está uma explicação detalhada sobre como o HTTP funciona dentro da camada de aplicação do modelo TCP/IP:

[Uma visão geral do HTTP - HTTP | MDN](#9)

### Funcionamento do HTTP

1. **Cliente e Servidor**: O HTTP segue um modelo cliente-servidor. O cliente (geralmente um navegador web) envia uma solicitação HTTP para um servidor web, que então processa a solicitação e envia de volta uma resposta HTTP.
1. **Mensagens HTTP**: Existem dois tipos principais de mensagens HTTP:
- **Solicitações (Requests)**: Enviadas pelo cliente ao servidor. Elas contêm um método HTTP (como GET, POST, PUT, DELETE), a URL do recurso solicitado, e, possivelmente, cabeçalhos e corpo da solicitação.
- **Respostas (Responses)**: Enviadas pelo servidor de volta ao cliente. Elas contêm um código de status (como 200 OK, 404 Not Found), cabeçalhos de resposta, e o corpo da resposta, que pode incluir o conteúdo solicitado (como uma página HTML).
1. **Métodos HTTP**:
- **GET**: Recupera, recebe dados de um servidor. É usado para solicitar um recurso específico.
- **POST**: Envia dados ao servidor, geralmente para criar ou atualizar um recurso.
- **PUT**: Atualiza um recurso existente ou cria um novo recurso no servidor.
- **DELETE**: Remove um recurso específico no servidor.
- Outros métodos incluem HEAD, OPTIONS, PATCH, etc.
1. **URLs e URIs**: Cada recurso na web é identificado por um URL (Uniform Resource Locator), que é uma forma específica de URI (Uniform Resource Identifier). A URL inclui o esquema (como http ou https), o nome do host (como [www.example.com](http://www.example.com/)), e o caminho do recurso (como /index.html).
1. **Cabeçalhos HTTP**: As mensagens HTTP contêm cabeçalhos que fornecem informações adicionais sobre a solicitação ou resposta. Por exemplo, cabeçalhos podem indicar o tipo de conteúdo sendo enviado (Content-Type), o tamanho do conteúdo (Content-Length), informações de cache (Cache-Control), entre outros.

### Exemplos de Operações HTTP

1. **Solicitação GET**:
- O cliente envia: `GET /index.html HTTP/1.1`
- O servidor responde com a página HTML solicitada.
1. **Solicitação POST**:
- O cliente envia: `POST /submit-form HTTP/1.1` junto com os dados do formulário no corpo da solicitação
- O servidor processa os dados e envia uma resposta apropriada.

### Como o HTTP se Encaixa no Modelo TCP/IP

- **Camada de Aplicação**: O HTTP opera na camada de aplicação do modelo TCP/IP, utilizando a infraestrutura fornecida pelas camadas inferiores.
- **Camada de Transporte**: O HTTP geralmente utiliza o protocolo TCP na camada de transporte para garantir a entrega confiável das mensagens.
- **Camada de Internet**: O TCP, por sua vez, utiliza o protocolo IP (Internet Protocol) para rotear as mensagens entre o cliente e o servidor através da rede.
- **Camada de Enlace de Dados**: Finalmente, o IP utiliza protocolos da camada de enlace de dados para transmitir os pacotes pela rede física.

### Conclusão

O HTTP é um protocolo essencial para a web moderna, operando na camada de aplicação do modelo TCP/IP. Ele define como os clientes e servidores se comunicam, permitindo a transferência de recursos como páginas web e arquivos multimídia. Compreender o HTTP é fundamental para o desenvolvimento e a utilização de aplicações web.
