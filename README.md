# GEF-BioTag - IOT

GEF-BioTag é uma solução desenvolvida para a disciplina de Arquiteturas Disruptivas, com foco em Internet das Coisas (IoT) e Inteligência Artificial Generativa. O objetivo é facilitar o registro, identificação e acompanhamento de pacientes em situações de emergência, utilizando pulseiras NFC integradas ao monitoramento de dados vitais via IoT.

## Funcionalidades

- Registro de pacientes com identificação por pulseira NFC
- Simulação de leitura NFC para testes
- Consulta e edição de informações dos pacientes
- Visualização de abrigos disponíveis e seus pacientes
- Monitoramento de batimentos cardíacos dos pacientes em tempo real
- Modal de informações sobre equipe, termos de uso, sobre o app e ajuda
- Integração com API para persistência dos dados

## Estrutura dos Dados

O backend fornece um arquivo JSON ([pacientes.json](pacientes.json)) que representa os pacientes cadastrados. Cada paciente possui informações pessoais, endereço, dados do abrigo, pulseira NFC e monitoramento cardíaco. 

**Exemplo de estrutura NFC no JSON:**
```json
{
  "id": "1",
  "name": "Maria Silva",
  "address": "Rua maria antônia ",
  "bracelet": {
    "id": "NFC000123",
    "nfc": {
      "id": "NFC000123",
      "information": [
        "Nome: Maria Silva",
        "Abrigo: Igreja São Francisco"
      ]
    },
    "iotHeartRate": {
      "id": "HR000123",
      "bpm": 80,
      "timestamp": 1749133335943
    }
  },
  "shelterId": "shelter-5",
  "createdAt": 1717510000000,
  "updatedAt": 1749133335943
}
```
**Destaque:**
A pulseira NFC contém um campo id e um array information com os dados do paciente, permitindo rápida identificação e acesso às informações essenciais em situações críticas.

**Equipe**
Eduardo Henrique Strapazzon Nagado - RM558158
Felipe Silva Maciel - RM555307
Gustavo Ramires Lazzuri - RM556772

**Link da Apresentação**
Assista no YouTube: https://youtu.be/Frx5oA6V2Wg?si=pczefpLX0xAd4wab

**Termos de Uso**
Este aplicativo é destinado ao gerenciamento de pacientes em situações de emergência, utilizando identificação por pulseira NFC. O uso é restrito a fins acadêmicos e demonstração. Nenhum dado real é coletado ou compartilhado.

**Ajuda**
Em caso de dúvidas, entre em contato:

- rm558158@fiap.com.br
- rm555307@fiap.com.br
- rm556772@fiap.com.br
