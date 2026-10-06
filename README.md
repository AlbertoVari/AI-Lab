# AI-Lab

**An index of Alberto Varignana's AI prototypes, experiments and engineering projects.**

This portfolio spans machine learning, computer vision, edge inference, multimodal GenAI, document retrieval, hybrid quantum/classical learning and governed agentic workflows. A recurring focus is connecting AI capabilities to business processes, APIs, cloud services and physical devices.

[GitHub profile](https://github.com/AlbertoVari) · [ProntoAgente website](https://prontoagente.it/)

## Start here

For a general AI Engineer review, start with these four complementary prototypes:

| Project | Engineering focus | Current scope |
| --- | --- | --- |
| [ProntoAgente.it](https://github.com/AlbertoVari/ProntoAgente.it) | Governed enterprise AI backend, robust process orchestration, and legacy ERP integration. | Production-ready architectural blueprint for secure email-to-ERP document processing. Implements strict Enterprise Governance via Role-Based Access Control (RBAC), multi-tenant isolation, versioned agentic workflows, and an approval-first execution pipeline. Features a resilient transactional outbox pattern for asynchronous workers, deterministic tool-call constraints, precise budget accounting, and immutable audit logs. Built with high-security constraints to ensure complete environment segregation and compliance before executing live target operations. |
| [Theoretical Physics Agent Lab](https://github.com/AlbertoVari/theoretical-physics-agent-lab) | Multi-agent orchestration, structured outputs and artifact handling | Research prototype with an offline test path |
| [Microsoft Learn MCP Client](https://github.com/AlbertoVari/microsoft-learn-mcp-client) | Tool discovery, document retrieval and source-grounded synthesis | Local client with tests; external services required for live use |
| [AI-GO-Game](https://github.com/AlbertoVari/AI-GO-Game) | Local multimodal models, camera input and speech | Hardware-dependent experimental application |

For business AI, also explore [Azure Foundry Agentic Supply Chain](https://github.com/AlbertoVari/azure-foundry-agentic-supply-chain). For training-oriented roles, see [PredictionMeta4](https://github.com/AlbertoVari/PredictionMeta4), [SolidQML](https://github.com/AlbertoVari/SolidQML) and [ML-RockPaperScissorsGame](https://github.com/AlbertoVari/ML-RockPaperScissorsGame), together with their methodological and reproducibility limits.

## How the projects are ordered

The catalog below runs from **lower to higher estimated engineering complexity**. The order considers model/training requirements, system components, hardware and cloud integration, orchestration, persistence, validation and operational controls. It is a qualitative guide: neighboring projects can be comparable, and specialized research may be difficult for reasons unrelated to system size.

**Complexity is not a production-readiness or quality score.** A larger prototype can still use simulated components. The descriptions distinguish implemented code, external pretrained services, mock behavior and planned integrations.

This repository is a navigation hub: it links to source repositories rather than copying them. Forks are listed separately with upstream attribution. No authorship of upstream frameworks is claimed. The catalog reflects a static review of the accessible default branches on **5 October 2026**; it does not certify that every project currently runs, that tests pass, or that a deployment is live.

## Prototype catalog — increasing complexity

### 1 — Focused experiments and AI integration demos

| # | Project | Area and stack | Prototype description and limits |
| --- | --- | --- | --- |
| 1 | [StarWars-ML-classification](https://github.com/AlbertoVari/StarWars-ML-classification) | **Image classification**<br>Jetson Nano | Small character-classification experiment. The repository currently contains labels and a command; training code and model artifacts are not included. |
| 2 | [ChatGPT](https://github.com/AlbertoVari/ChatGPT) | **LLM API experiments**<br>Python · OpenAI | Small scripts for conversational and social-content experiments. Includes legacy API usage that needs updating before reuse. |
| 3 | [AlphaFold-api](https://github.com/AlbertoVari/AlphaFold-api) | **AI data API integration**<br>Python · FastAPI · httpx | API wrapper for retrieving existing AlphaFold protein-structure predictions. Integrates an AI data service; it does not train or run AlphaFold. |
| 4 | [StockbuzzAI](https://github.com/AlbertoVari/StockbuzzAI) | **NLP and cloud data**<br>Python · Google Cloud Natural Language · BigQuery | Twitter sentiment-analysis script integrating managed NLP and cloud data storage. Historical API dependencies need verification. |
| 5 | [BrotherEye](https://github.com/AlbertoVari/BrotherEye) | **Browser computer vision**<br>TensorFlow.js · MobileNet · Web3 | Web demonstration combining pretrained image classification with blockchain registration. |
| 6 | [TokenML](https://github.com/AlbertoVari/TokenML) | **Edge AI and tokenization**<br>Web UI · edge inference integration | Experiment connecting image-detection outputs and tokenization. Minimal documentation; intended as an integration demo. |
| 7 | [GourmetAI](https://github.com/AlbertoVari/GourmetAI) | **NLP and blockchain integration**<br>Python · Web3 · pandas | Historical experiment linking sentiment data and Ethereum/Kaleido transactions. The published scripts demonstrate integration components rather than a complete packaged service. |
| 8 | [AI-TSE](https://github.com/AlbertoVari/AI-TSE) | **ERP anomaly checks**<br>Python · FastAPI · Pydantic · httpx | Warehouse-movement middleware returning ALLOW, WARN or BLOCK from explicit rules. Smart Services and historical profiles use mocks or indicative endpoints; no LLM or trained anomaly model is implemented in the inspected main file. |
| 9 | [JobSearch_Agent](https://github.com/AlbertoVari/JobSearch_Agent) | **Search and ranking automation**<br>Python · FastAPI · Google Custom Search | Job-search application with parsing and rule-based ranking. Salary benchmarks are placeholders; the inspected main file does not call an LLM. Packaging of templates/static assets needs completion. |
| 10 | [Tax-Advisor-NAVISION](https://github.com/AlbertoVari/Tax-Advisor-NAVISION) | **Finance-oriented LLM prototype**<br>Python · Gemini/Vertex AI · Gradio · Dockerfile | Prompt-led assistant for NAV/Business Central accounting drafts, exported from Vertex AI Studio. The inspected code includes tool specifications as prompt text, without demonstrated tool dispatch. Container packaging needs completion. |

### 2 — Model training and focused learning experiments

| # | Project | Area and stack | Prototype description and limits |
| --- | --- | --- | --- |
| 11 | [ML-RockPaperScissorsGame](https://github.com/AlbertoVari/ML-RockPaperScissorsGame) | **CNN image classification**<br>Python · TensorFlow/Keras · Jetson | Training and inference scripts for rock-paper-scissors recognition. Includes image augmentation and a CNN training workflow; environment and evaluation results need fuller documentation. |
| 12 | [PredictionMeta4](https://github.com/AlbertoVari/PredictionMeta4) | **Financial time-series ML**<br>Python · scikit-learn · TensorFlow/Keras | Collection of ANN, regression, Random Forest and quantum-inspired market-prediction experiments. Selected scripts need corrections to data scaling, residual modelling and evaluation before predictive results can be relied on. |

### 3 — Edge AI and multimodal applications

| # | Project | Area and stack | Prototype description and limits |
| --- | --- | --- | --- |
| 13 | [Pi-IoT-Vision](https://github.com/AlbertoVari/Pi-IoT-Vision) | **Edge inference and cloud ingestion**<br>Python · TensorFlow Lite · Coral TPU · Raspberry Pi | Image-recognition gateway combining local accelerated inference and cloud data collection. Requires the hardware and local dependencies described by the project. |
| 14 | [DeepStreamAI](https://github.com/AlbertoVari/DeepStreamAI) | **Video inference pipeline**<br>Python · NVIDIA DeepStream · GStreamer · Jetson | USB-camera vision pipeline using NVIDIA's inference stack. Focuses on deployment and pipeline integration rather than training a new model. |
| 15 | [MarketVision](https://github.com/AlbertoVari/MarketVision) | **OCR and market-display monitoring**<br>Python · OpenVINO · Tesseract · Raspberry Pi · Movidius | Reads market-display images and translates detected index changes into GPIO/LED alerts. This is an OCR/inference integration prototype, not a validated trading predictor. |
| 16 | [Edge-AI-face-detection](https://github.com/AlbertoVari/Edge-AI-face-detection) | **Distributed face recognition**<br>Python · Flask · OpenVINO · Raspberry Pi | Captures images on a Raspberry Pi, sends them to a laptop inference service and returns recognition results for local feedback. |
| 17 | [Deadmouse](https://github.com/AlbertoVari/Deadmouse) | **Hand tracking and interactive control**<br>Python · TensorFlow Lite · OpenVINO · Pygame | Uses hand landmarks and gesture models to control an on-screen pointer. Includes model assets and a demonstration video. |
| 18 | [Gorilla](https://github.com/AlbertoVari/Gorilla) | **Gesture-driven robotics**<br>Python · PyTorch · ONNX/TVM · Jetson · LEGO EV3 | Combines Temporal Shift Module gesture inference with robot control. Demonstrates integration across vision models, accelerated inference and physical actuation. |
| 19 | [AI-GO-Game](https://github.com/AlbertoVari/AI-GO-Game) | **Local multimodal GenAI**<br>Python · Ollama/LangChain · Qwen vision · Whisper · Piper | Go-playing assistant combining camera input, a vision-language model, speech recognition and speech synthesis. Requires a suitable local model and audio/video environment. |

### 4 — Hybrid research and document-grounded assistants

| # | Project | Area and stack | Prototype description and limits |
| --- | --- | --- | --- |
| 20 | [SolidQML](https://github.com/AlbertoVari/SolidQML) | **Hybrid quantum/classical ML**<br>Python · PyTorch · Qiskit · Jetson · IBM Quantum | Hybrid neural-network experiments combining classical layers and quantum circuits, including MNIST classification. Published code uses historical dependencies; reproducible setup and comparative metrics should be documented. |
| 21 | [QuantumBioinformatic](https://github.com/AlbertoVari/QuantumBioinformatic) | **Quantum bioinformatics experiment**<br>Jupyter Notebook · PennyLane | Educational notebook connecting genetic-sequence features, simulated mutations and quantum-state similarity. Exploratory research, without established biological predictive validity. |
| 22 | [Qtsumego](https://github.com/AlbertoVari/Qtsumego) | **Variational quantum learning**<br>Python · Qiskit · NumPy | Hybrid quantum/classical research prototype for Go life-and-death analysis using parameterized circuits, Born-machine concepts and classical board logic. |
| 23 | [microsoft-learn-mcp-client](https://github.com/AlbertoVari/microsoft-learn-mcp-client) | **Document retrieval and LLM synthesis**<br>Python · MCP · JSON Schema · OpenAI Responses API | Discovers Microsoft Learn tools, validates arguments, retrieves documentation and synthesizes sourced answers in Italian. Includes protocol and synthesis tests. Retrieval uses an external MCP service; this is not a custom vector-database pipeline. |
| 24 | [QISKIT-code](https://github.com/AlbertoVari/QISKIT-code) | **Quantum experiments including QML**<br>Python · Qiskit | Broader quantum-computing collection with an AI-related fraud-detection QML example. Included here for its QML component; most of the repository concerns quantum algorithms rather than AI engineering. |

### 5 — Orchestrated workflows and governed AI platforms

| # | Project | Area and stack | Prototype description and limits |
| --- | --- | --- | --- |
| 25 | [azure-foundry-agentic-supply-chain](https://github.com/AlbertoVari/azure-foundry-agentic-supply-chain) | **Business multi-agent workflow**<br>Python · Azure AI Foundry · Azure AI Search · GPT models | Procurement prototype coordinating BOM extraction, inventory checks, supplier selection and purchase-order drafting. Prompt definitions and a sequential orchestrator are published; REST endpoints, tool schemas and response parsing require environment-specific adaptation. |
| 26 | [theoretical-physics-agent-lab](https://github.com/AlbertoVari/theoretical-physics-agent-lab) | **Scientific multi-agent workflow**<br>Python · OpenAI Agents SDK · Pydantic · Code Interpreter | Three-role workflow that turns a paper into an experiment protocol, generated simulation artifacts and an evidence review. Includes structured outputs, checkpoints, retries, artifact transfer and offline tests. Research prototype; local AST checks are not a complete sandbox. |
| 27 | [ProntoAgente.it](https://github.com/AlbertoVari/ProntoAgente.it) | **Governed enterprise AI backend**<br>Python · FastAPI · SQLAlchemy · Alembic · Pydantic | Multi-tenant prototype for email-to-ERP proposals with RBAC, versioned workflows, approval-first execution, outbox workers, constrained tool calls, budget accounting and audit records. The M3 showcase is offline: provider fake, synthetic mailbox and simulated ERP. The OpenAI adapter is opt-in and not live-validated; production is explicitly blocked. |

## Architecture companion

[**architettura-impresa-agentica**](https://github.com/AlbertoVari/architettura-impresa-agentica) proposes a reference architecture for governed enterprise agents across data, SQL, ERP, user experience, processes and business strategy. It contains a manifesto, diagrams and an adoption roadmap. It is design documentation rather than an executable implementation, so it is kept outside the complexity ranking.

## Forks and learning references

These repositories are upstream projects forked for exploration or reference. Their complexity belongs to the upstream implementation and is **not evidence that I built the original framework**. The list is broadly grouped from examples to model/deployment infrastructure and research platforms; it is not a ranking of my contribution.

| Fork | Area | Upstream | Purpose |
| --- | --- | --- | --- |
| [Twitter-Sentiment-Analysis-with-TensorFlow](https://github.com/AlbertoVari/Twitter-Sentiment-Analysis-with-TensorFlow) | NLP | [MustafaWaheed91/Twitter-Sentiment-Analysis-with-TensorFlow](https://github.com/MustafaWaheed91/Twitter-Sentiment-Analysis-with-TensorFlow) | TensorFlow sentiment-analysis example |
| [amazon-forecast-samples](https://github.com/AlbertoVari/amazon-forecast-samples) | Forecasting | [aws-samples/amazon-forecast-samples](https://github.com/aws-samples/amazon-forecast-samples) | Amazon Forecast notebooks and examples |
| [training-data-analyst](https://github.com/AlbertoVari/training-data-analyst) | Cloud ML | [GoogleCloudPlatform/training-data-analyst](https://github.com/GoogleCloudPlatform/training-data-analyst) | Google Cloud training labs and demos |
| [chatgpt_telegram_bot](https://github.com/AlbertoVari/chatgpt_telegram_bot) | LLM applications | [father-bot/chatgpt_telegram_bot](https://github.com/father-bot/chatgpt_telegram_bot) | Telegram bot integrating LLM services |
| [taureau](https://github.com/AlbertoVari/taureau) | NLP/finance | [tahmidrashid/taureau](https://github.com/tahmidrashid/taureau) | Market-movement inference from Twitter sentiment |
| [disentanglement_lib](https://github.com/AlbertoVari/disentanglement_lib) | Representation learning | [google-research/disentanglement_lib](https://github.com/google-research/disentanglement_lib) | Research library for disentangled representations |
| [qnn_builder_pennylane](https://github.com/AlbertoVari/qnn_builder_pennylane) | Quantum ML | [mahabubul-alam/qnn_builder_pennylane](https://github.com/mahabubul-alam/qnn_builder_pennylane) | Quantum neural-network construction scripts |
| [Deakin_Quantum-ML_genomic](https://github.com/AlbertoVari/Deakin_Quantum-ML_genomic) | Quantum ML | [PokhrelDeakinGitHub/Deakin_Quantum-ML_genomic](https://github.com/PokhrelDeakinGitHub/Deakin_Quantum-ML_genomic) | Quantum ML experiments for genomic data |
| [temporal-shift-module](https://github.com/AlbertoVari/temporal-shift-module) | Video learning | [mit-han-lab/temporal-shift-module](https://github.com/mit-han-lab/temporal-shift-module) | Temporal Shift Module video-understanding implementation |
| [V2V-PoseNet_RELEASE](https://github.com/AlbertoVari/V2V-PoseNet_RELEASE) | Pose estimation | [mks0601/V2V-PoseNet_RELEASE](https://github.com/mks0601/V2V-PoseNet_RELEASE) | Voxel-to-voxel 3D pose-estimation implementation |
| [jetson-inference](https://github.com/AlbertoVari/jetson-inference) | Edge deployment | [dusty-nv/jetson-inference](https://github.com/dusty-nv/jetson-inference) | Jetson inference tutorials and vision primitives |
| [ncsdk](https://github.com/AlbertoVari/ncsdk) | Inference infrastructure | [movidius/ncsdk](https://github.com/movidius/ncsdk) | Movidius Neural Compute Stick software development kit |
| [openvino](https://github.com/AlbertoVari/openvino) | Inference infrastructure | [openvinotoolkit/openvino](https://github.com/openvinotoolkit/openvino) | Toolkit for optimizing and deploying inference |
| [PINTO_model_zoo](https://github.com/AlbertoVari/PINTO_model_zoo) | Model conversion | [PINTO0309/PINTO_model_zoo](https://github.com/PINTO0309/PINTO_model_zoo) | Models converted across inference frameworks |
| [AI-Scientist](https://github.com/AlbertoVari/AI-Scientist) | Agentic research | [SakanaAI/AI-Scientist](https://github.com/SakanaAI/AI-Scientist) | Automated scientific-discovery research framework |
| [Qwen3.6](https://github.com/AlbertoVari/Qwen3.6) | Vision/language models | [QwenLM/Qwen3.8](https://github.com/QwenLM/Qwen3.8) | Fork of the Qwen model-series repository |

## What this portfolio demonstrates

- **Python and API integration:** services and prototypes built around FastAPI, HTTP clients and structured data contracts.
- **ML and inference:** examples using scikit-learn, TensorFlow/Keras, PyTorch, TensorFlow Lite, OpenVINO and NVIDIA tooling.
- **LLM applications:** prompt-led assistants, source-grounded synthesis, local multimodal models and agent orchestration.
- **Workflow engineering:** structured outputs, checkpoints, artifact handling, explicit failure states and human approval in the projects that implement them.
- **Business context:** experiments around ERP, procurement, administration, document processing and finance.

The portfolio does not imply uniform experience across every framework or a production deployment for every prototype. Project-specific code, tests, setup instructions and limitations are the evidence for each capability.

## Scope and related work

The catalog contains **27 implementation/experiment repositories**, **one architecture companion** and **16 AI-related forks or infrastructure references**. Small search utilities without an AI model, pure blockchain projects and purely quantum algorithms are outside this AI catalog. The QML-containing QISKIT-code collection is included with its scope made explicit.

Private or empty repositories are not offered as public portfolio evidence.

## Exploring a project

Follow the repository link for source code and environment instructions. Hardware projects require their specified devices; cloud and LLM projects may require credentials and paid services. Offline mock results demonstrate software behavior within the mock environment and should not be interpreted as live-provider, customer or model-quality benchmarks.

For questions about a prototype, its implementation choices or collaboration, contact me through the channels on my [GitHub profile](https://github.com/AlbertoVari).
