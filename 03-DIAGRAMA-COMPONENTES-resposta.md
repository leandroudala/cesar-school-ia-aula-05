# 📘 Diagrama de Componentes - PROTEC (PlantUML)
A PROTEC deseja modernizar seus sistemas por meio de Inteligência Artificial, atuando em três principais frentes:
- Automação Inteligente de Processos
- Análise Preditiva e Apoio à Decisão
- Otimização de Infraestrutura e Segurança Cibernética

Este diagrama reflete essa estrutura modular e sua interação com sistemas legados e usuários.

# 🔧 PlantUML - Código

```plantuml
@startuml
' Estilo visual
skinparam componentStyle rectangle
skinparam defaultTextAlignment center

title Diagrama de Componentes - PROTEC e Soluções de IA

package "PROTEC - Núcleo de Sistemas" {
    [Portal de Serviços Públicos]
    [Sistemas de Benefícios Sociais]
    [Gestão de Chamados]
    [Central de Documentos]
    [Data Warehouse Governamental]
    [Infraestrutura de TI]
}

package "Módulos de Inteligência Artificial" {
    [IA de Classificação de Documentos] as DocIA
    [IA de Atendimento (Chatbot)] as ChatIA
    [IA de Triagem de Chamados] as ChamadoIA
    [IA de Análise de Conformidade] as ConformIA

    [IA Preditiva de Demanda] as PrevisaoIA
    [IA de Detecção de Fraudes] as FraudeIA
    [IA de Dashboards Inteligentes] as DashIA

    [IA de Monitoramento de Infraestrutura] as MonitorIA
    [IA de Otimização de Recursos] as RecursoIA
    [IA de Segurança Cibernética] as SegurancaIA
}

actor "Servidor Público" as Servidor
actor "Cidadão" as Cidadao

' Atores e interações
Servidor --> [Portal de Serviços Públicos]
Cidadao --> [Portal de Serviços Públicos]

' Integrações dos sistemas com módulos de IA
[Central de Documentos] --> DocIA
[Portal de Serviços Públicos] --> ChatIA
[Gestão de Chamados] --> ChamadoIA
[Sistemas de Benefícios Sociais] --> ConformIA

[Data Warehouse Governamental] --> PrevisaoIA
[Data Warehouse Governamental] --> FraudeIA
[Data Warehouse Governamental] --> DashIA

[Infraestrutura de TI] --> MonitorIA
[Infraestrutura de TI] --> RecursoIA
[Infraestrutura de TI] --> SegurancaIA

' Relacionamentos internos
PrevisaoIA --> DashIA
FraudeIA --> DashIA
MonitorIA --> RecursoIA

@enduml
```

# 🔗 Referência
Você pode visualizar este código diretamente no site do PlantUML:
👉 https://plantuml.com/component-diagram

Se quiser, posso gerar a imagem para você. Deseja isso?