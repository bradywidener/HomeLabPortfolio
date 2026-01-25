# sdvd-node2

### Specifications
> Model
> - Lenovo Tiny ThinkCentre P320

> Operating System
> - Proxmox VE 9.1.1

> CPU - Intel i5-6500T
> - 4 Cores
> -  4 Threads
> - 2.5 GHz Base Frequency

> Memory
> - 32GB (2x16GB SODDR4)

> Storage
> - 64GB Flashdrive (for OS)
> - 250GB NVMe (VM Storage)
> - 250GB NVMe (VM Storage)

> Graphics
> - NVIDIA Quadro P600

### Containers and VMs
> sdvd-ai
> - This VM hosts my local LLM's I have running with Ollama. Currently I'm using two different versions of Qwent2.5. One with 3 billion paramaters, and one with 7 billion paramters. With my specs being lower for AI workloads, this is more of a 'show and tell' project, than something that is actually practical. 
> sdvd-mcp
> - This VM hosts my Open WebUI front end for my AI models. I also plan to use this VM to run various MCP servers for my LLMs.