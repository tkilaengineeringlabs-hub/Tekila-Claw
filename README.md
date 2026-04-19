Tekila-Claw — Personal AI Architect & Assistant
Tekila-Claw es el asistente de inteligencia artificial personal de Tekila Engineering Labs, diseñado para operar de forma autónoma en hardware propio. Centraliza la comunicación, automatiza tareas de ingeniería y actúa como el plano de control (Control Plane) para todos nuestros sistemas.

Ecosistema de Comunicación
El asistente opera de forma transparente en los canales que ya utilizamos diariamente, permitiendo una gestión fluida sin cambiar de plataforma:

Mensajería: WhatsApp, Telegram, Signal, iMessage.

Colaboración: Slack, Discord, Microsoft Teams, Google Chat.

Avanzado: Matrix, Nostr, WebChat.

Instalación y Setup (Rápido)
El entorno requiere Node ≥22. La configuración se realiza mediante el asistente de arquitectura de Tekila:

Bash
# Instalación global del núcleo de Tekila-Claw
npm install -g @tekila-labs/claw@latest

# Iniciar el asistente de configuración (Daemon install)
tekila-claw onboard --install-daemon
Comandos de Control Rápido
Bash
# Iniciar el Gateway (Control Plane) en modo verbose
tekila-claw gateway --port 18789 --verbose

# Enviar una notificación de sistema a través de los canales conectados
tekila-claw message send --to "Jesus Figueroa" --message "Deployment de Autoware completado."

# Consultar al agente con nivel de pensamiento profundo (Thinking Mode)
tekila-claw agent --message "Revisar arquitectura de red para BioMaker Labs" --thinking high
Capacidades de Ingeniería (Highlights)
Local-first Gateway: Control total sobre sesiones, herramientas y eventos sin depender de nubes externas.

Multi-agent Routing: Capacidad para aislar agentes por proyecto (Master Coat, Sazón de Barrio, Mini Maker Labs).

Voice & Talk Mode: Activación por voz (Wake words) en iOS/Android y síntesis avanzada (ElevenLabs).

Live Canvas: Espacio visual interactivo impulsado por la IA para diseño de arquitectura en tiempo real.

Sandbox Security: Ejecución segura de código (bash/python) en contenedores Docker aislados.

Comandos de Chat (Directos en la App)
Puedes controlar el comportamiento del asistente directamente desde WhatsApp o Slack con estos comandos:

/status — Estado de la sesión, modelo activo y consumo.

/new — Resetear la memoria de la sesión actual.

/think <level> — Ajustar potencia de razonamiento (off | low | medium | high | xhigh).

/usage tokens — Ver estadísticas de consumo de la API.

/activation mention — Cambiar modo de activación (Solo mención o siempre activo).

Arquitectura de Operación
Canales (WhatsApp / Telegram / Slack / Discord)
               │
               ▼
┌───────────────────────────────┐
│       Tekila Gateway          │
│      (Control Plane)          │
│    ws://127.0.0.1:18789       │
└──────────────┬────────────────┘
               │
               ├─ Pi Agent (Lógica de IA)
               ├─ CLI Interface
               ├─ WebChat UI (Dashboard)
               ├─ Nodes (Cámaras, Sensores, GPS)
               └─ Tekila-Claw Mobile App
Sobre este Proyecto
Este asistente es el núcleo operativo de Tekila Engineering Labs, enfocado en la eficiencia, la privacidad de datos y la automatización creativa.

Lead Architect: Jesús Figueroa (Txus)

Visión: Ingeniería responsable y autonomía tecnológica.

Tekila Engineering Labs
Destilando tecnología, refinando el futuro.
