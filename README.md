## Spring AI Demo

using `llama 2` embeddings and `pgvector` for similarity search, `openai` for text generation

> PS:
> `llama` embedding 4096 dimension
> `openai text-embedding-ada-002` embedding 1536 dimension (spring-ai-core-0.8.0-SNAPSHOT.jar!/embedding/embedding-model-dimensions.properties)

```shell
curl http://localhost:11434/api/embeddings -d '{
  "model": "llama2",
  "prompt": "Here is an article about llamas..."
}' | jq '.embedding | length'
```

## Reference

* https://github.com/ollama/ollama
* https://docs.spring.io/spring-ai/reference/api/embeddings/ollama-embeddings.html
* https://docs.spring.io/spring-ai/reference/api/vectordbs/pgvector.html
* https://github.com/spring-tips/llm-rag-with-spring-ai
*

## Config

* `SPRING_AI_OPENAI_API_KEY`
* `SPRING_AI_OPENAI_BASE_URL`

```shell
export SPRING_AI_OPENAI_API_KEY=<INSERT KEY HERE>
```

