# HTTP Status Codes

## 1xx Informational
- **100 Continue**: O servidor recebeu a solicitação inicial e o cliente deve continuar com a solicitação.
- **101 Switching Protocols**: O servidor está mudando os protocolos conforme solicitado pelo cliente.
- **102 Processing (WebDAV)**: O servidor recebeu a solicitação e está processando-a, mas ainda não há resposta disponível.

## 2xx Success
- **200 OK**: A solicitação foi bem-sucedida.
- **201 Created**: A solicitação foi bem-sucedida e um novo recurso foi criado.
- **202 Accepted**: A solicitação foi recebida, mas ainda não foi executada.
- **203 Non-Authoritative Information**: A solicitação foi bem-sucedida, mas a resposta contém informações não originais.
- **204 No Content**: A solicitação foi bem-sucedida, mas não há conteúdo para enviar na resposta.
- **205 Reset Content**: A solicitação foi bem-sucedida, e o usuário deve redefinir o formulário visual.
- **206 Partial Content**: O servidor está entregando apenas parte do recurso devido a uma solicitação de intervalo.
- **207 Multi-Status (WebDAV)**: A mensagem do corpo é um XML que pode conter uma série de códigos de resposta, dependendo de quantas sub-solicitações foram feitas.
- **208 Already Reported (WebDAV)**: Os membros de um conjunto de ligações DAV já foram enumerados em uma resposta anterior.
- **226 IM Used**: O servidor concluiu a solicitação para o recurso, e a resposta é uma representação do resultado de uma ou mais instâncias de manipulação aplicada ao recurso atual.

## 3xx Redirection
- **300 Multiple Choices**: Existem várias opções para o recurso que o cliente pode seguir.
- **301 Moved Permanently**: O recurso solicitado foi movido permanentemente para um novo URI.
- **302 Found**: O recurso solicitado foi encontrado, mas está temporariamente em um local diferente.
- **303 See Other**: O cliente deve usar um URI diferente para acessar o recurso solicitado.
- **304 Not Modified**: O recurso não foi modificado desde a última solicitação.
- **305 Use Proxy**: O recurso solicitado deve ser acessado através de um proxy.
- **306 Switch Proxy**: Código de status não utilizado atualmente, mas reservado para uso futuro.
- **307 Temporary Redirect**: O recurso solicitado está temporariamente em um local diferente, mas o cliente deve usar o URI original para futuras solicitações.
- **308 Permanent Redirect**: O recurso solicitado foi movido permanentemente para um novo URI, e o cliente deve usar o URI fornecido para futuras solicitações.

## 4xx Client Errors
- **400 Bad Request**: A solicitação não pôde ser entendida pelo servidor devido à sintaxe incorreta.
- **401 Unauthorized**: A solicitação requer autenticação do usuário.
- **402 Payment Required**: Reservado para uso futuro.
- **403 Forbidden**: O servidor entendeu a solicitação, mas se recusa a autorizá-la.
- **404 Not Found**: O servidor não encontrou o recurso solicitado.
- **405 Method Not Allowed**: O método especificado na solicitação não é permitido para o recurso identificado.
- **406 Not Acceptable**: O recurso solicitado é capaz de gerar apenas conteúdo não aceitável de acordo com os cabeçalhos Accept enviados na solicitação.
- **407 Proxy Authentication Required**: O cliente deve primeiro se autenticar com o proxy.
- **408 Request Timeout**: O servidor esgotou o tempo limite enquanto aguardava a solicitação.
- **409 Conflict**: A solicitação não pôde ser concluída devido a um conflito com o estado atual do recurso.
- **410 Gone**: O recurso solicitado não está mais disponível e não será disponibilizado novamente.
- **411 Length Required**: O servidor recusou a solicitação porque o cabeçalho Content-Length não está definido.
- **412 Precondition Failed**: Uma ou mais condições especificadas nos cabeçalhos da solicitação foram avaliadas como falsas pelo servidor.
- **413 Payload Too Large**: A solicitação é maior do que o servidor pode processar.
- **414 URI Too Long**: O URI fornecido na solicitação é muito longo para ser processado pelo servidor.
- **415 Unsupported Media Type**: O formato de mídia da solicitação não é suportado pelo servidor.
- **416 Range Not Satisfiable**: O intervalo especificado pelo cabeçalho Range na solicitação não pode ser satisfeito.
- **417 Expectation Failed**: O servidor não pode atender aos requisitos do campo Expect da solicitação.
- **418 I'm a teapot**: Código definido no RFC 2324, Hyper Text Coffee Pot Control Protocol. Esta é uma piada de 1º de abril.
- **421 Misdirected Request**: A solicitação foi direcionada a um servidor que não pode produzir uma resposta.
- **422 Unprocessable Entity (WebDAV)**: A solicitação estava bem formada, mas não pôde ser seguida devido a erros semânticos.
- **423 Locked (WebDAV)**: O recurso que está sendo acessado está bloqueado.
- **424 Failed Dependency (WebDAV)**: A solicitação falhou devido à falha de uma solicitação anterior.
- **425 Too Early**: O servidor não está disposto a arriscar processar uma solicitação que pode ser repetida.
- **426 Upgrade Required**: O cliente deve mudar para um protocolo diferente, conforme indicado no cabeçalho Upgrade.
- **428 Precondition Required**: O servidor exige que a solicitação seja condicional.
- **429 Too Many Requests**: O usuário enviou muitas solicitações em um determinado tempo.
- **431 Request Header Fields Too Large**: Os campos de cabeçalho da solicitação são muito grandes.
- **451 Unavailable For Legal Reasons**: O recurso solicitado não está disponível por motivos legais.

## 5xx Server Errors
- **500 Internal Server Error**: O servidor encontrou uma condição inesperada que impediu a conclusão da solicitação.
- **501 Not Implemented**: O servidor não suporta a funcionalidade necessária para atender a solicitação.
- **502 Bad Gateway**: O servidor, ao atuar como gateway ou proxy, recebeu uma resposta inválida do servidor upstream.
- **503 Service Unavailable**: O servidor está atualmente indisponível (por sobrecarga ou manutenção).
- **504 Gateway Timeout**: O servidor, ao atuar como gateway ou proxy, não recebeu uma resposta oportuna do servidor upstream.
- **505 HTTP Version Not Supported**: O servidor não suporta a versão do protocolo HTTP usada na solicitação.
- **506 Variant Also Negotiates**: O servidor possui uma configuração interna de erro: o recurso não está disponível.
- **507 Insufficient Storage (WebDAV)**: O servidor não consegue armazenar a representação necessária para completar a solicitação.
- **508 Loop Detected (WebDAV)**: O servidor detectou um loop infinito ao processar a solicitação.
- **510 Not Extended**: A política de extensão para o recurso não está cumprida.
- **511 Network Authentication Required**: O cliente precisa se autenticar para ganhar acesso à rede.

