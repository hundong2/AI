# AI
agent, llm, rag, adk, mcp, langchain, a2a, langgraph


## 추론 모델

- o3, o4-mini, Gemini 2.5 pro, opus 4(옵션으로 추론 가능)
- 추론 모델의 경우 속도가 느림

## ollama 

- install `ollama` 

### setting gpu for nvidia

```sh
curl -fsSL https://nvidia.github.io/libnvidia-container/gpgkey | sudo gpg --dearmor -o /usr/share/keyrings/nvidia-container-toolkit-keyring.gpg
curl -s -L https://nvidia.github.io/libnvidia-container/stable/ubuntu18.04/nvidia-container-toolkit.list | \
sed 's#deb https://#deb [signed-by=/usr/share/keyrings/nvidia-container-toolkit-keyring.gpg] https://#g' | \
sudo tee /etc/apt/sources.list.d/nvidia-container-toolkit.list
sudo apt-get update
sudo apt-get install -y nvidia-container-toolkit
```

### run docker 

```sh
sudo systemctl restart docker
docker run -d --gpus=all -v ollama:/root/.ollama -p 11434:11434 --name ollama ollama/ollama
```

### embedding model install 

```sh
docker exec -it ollama ollama run nomic-embed-text
```