import JSON to N8N
use web apache or xampp edit *.html 
change <webhook> to your webhook url

install ollama install model 
change url ollama in llm model

news feed api by alientvault to LLM send chat Discord

<img src="https://img2.pic.in.th/pic/1ffe7a34458c41226.png" alt="1" border="0">

run n8n public IP with docker

> docker run -d --name n8n \\
  -p 5678:5678 \\
  -v n8n_data:/home/node/.n8n \\
  -e N8N_PROTOCOL=http \\
  -e N8N_HOST=0.0.0.0 \\
  -e N8N_PORT=5678 \\
  -e N8N_SECURE_COOKIE=false \\
  docker.n8n.io/n8nio/n8n start

run ollama public IP \
mac & linux

> OLLAMA_HOST=0.0.0.0 ollama serve

windows
use powershell

> $env:OLLAMA_HOST="<"IP Address">" \
> ollama serve

allow firewall everyone use

> New-NetFirewallRule -DisplayName "Allow Ollama" -Direction Inbound -Protocol TCP -LocalPort 11434 -Action Allow

powershell n8n public IP
 docker run -it --rm `
>>   -p 5678:5678 `
>>   -e N8N_HOST=0.0.0.0 `
>>   -e N8N_PORT=5678 `
>>   -e N8N_PROTOCOL=http `
>>   n8nio/n8n
