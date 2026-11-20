# Strands Avanzado: multi-agente, hooks y steering

Material del workshop **Strands Avanzado** del Student Builder Group de la Universidad Austral (20/11/2026).

Dos notebooks con ejemplos en español sobre un caso que todos entendemos: **organizar un viaje**. Las tools usan **datos inventados**: no hace falta ninguna API externa, solo acceso a un modelo en Amazon Bedrock.

| Notebook | Qué vas a ver |
|---|---|
| [`patrones-multiagente.ipynb`](patrones-multiagente.ipynb) | Los 5 patrones multi-agente: Agents as Tools, Swarm, Graph, Workflow y A2A |
| [`hooks-steering.ipynb`](hooks-steering.ipynb) | Cómo observar, bloquear y corregir al agente: Hooks, Interventions y Steering |

La presentación está en la carpeta [`presentacion/`](presentacion/).

## Requisitos

- Python 3.10 o superior.
- Una cuenta de AWS con acceso a Amazon Bedrock y al modelo Claude Haiku 4.5 (`us.anthropic.claude-haiku-4-5-20251001-v1:0`) en `us-east-1`.
- Credenciales configuradas con la AWS CLI (`aws configure` o `aws configure sso`).

## Cómo correrlo

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

Por defecto los notebooks usan tu perfil de AWS por defecto (`AWS_PROFILE = None`). Si querés usar un perfil con nombre, ponelo en `AWS_PROFILE` en la celda de setup de cada notebook. Si querés usar otro modelo o región, cambiá `MODEL_ID` y `REGION` en la misma celda.

## Recursos

- [Strands Agents](https://strandsagents.com)
- [Strands Agents en GitHub](https://github.com/strands-agents)
