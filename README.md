#OpenTracing com Kong e num futuro não tão próximo, Traefik.

Neste repo irei montar uma estrutura de Kong, Jaeger e Zipkin. Tanto o Jaeger quanto o Zipkin(?) nos entregam plataformas de tracing ou sampling de aplicações web e suas dependências. Com elas podemos acompanhar todos os passos, microservicos, bancos, apis e etc, que nossa aplicação utilzia.

O Kong é um gerenciador de api's/microservicos. Ele tem um plugin que utiliza o protocolo de tracing do Zipkin, que o Jaeger também aceita, para fins de compatibilidade.
O ideal é subir os serviços na seguinte ordem: Jaeger, Zipkin, Traefik, kong.-- 