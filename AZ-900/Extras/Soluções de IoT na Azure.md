
## 📡 O que é IoT (Internet of Things)?

A Internet das Coisas refere-se à rede de dispositivos físicos ("coisas") conectados que coletam e trocam dados com a nuvem. Esses dispositivos possuem sensores e capacidade de computação, variando desde termostatos inteligentes até sensores industriais e veículos.

Na AZ-900, você precisa saber diferenciar **três serviços principais** da Azure para IoT:

---

## 1. Azure IoT Hub

É o serviço central (um _hub_ de mensagens) que atua como o ponto de comunicação bidirecional entre os aplicativos (nuvem) e os dispositivos IoT.

- **Modelo:** **PaaS** (Plataforma como Serviço).
- **Foco:** Fornece o "motor" de comunicação. É ideal quando você precisa de controle total e tem uma equipe de desenvolvedores para criar o painel de controle e a solução do zero.
- **Características Principais:**
    - Suporta comunicação de milhões de dispositivos simultaneamente.
    - Permite enviar comandos da nuvem para o dispositivo (ex: "reiniciar máquina").
    - Roteamento de mensagens e integração nativa com outros serviços Azure.
        

## 2. Azure IoT Central

É uma solução pronta para uso (gerenciada) construída _sobre_ o IoT Hub, mas com uma interface gráfica amigável e painéis pré-configurados.

- **Modelo:** **SaaS** (Software como Serviço).
- **Foco:** Facilidade de uso e rapidez na implementação. Ideal quando você não quer (ou não tem tempo para) desenvolver a interface de gerenciamento do zero.
- **Características Principais:**
    - Dashboard web pronto (arrastar e soltar).
    - Templates por setor (ex: saúde, varejo, energia).
    - Conecta dispositivos e gerencia telemetria sem necessidade de código profundo.

## 3. Azure Sphere

É uma solução focada estritamente na **segurança de ponta a ponta** para dispositivos IoT conectados à internet.

- **Foco:** Garantir que o hardware e a comunicação do dispositivo não sejam hackeados.
- **Composição (A Tríade do Sphere):**
    1. **Azure Sphere MCU:** Microcontrolador (hardware) certificado e seguro construído nos dispositivos.
    2. **Azure Sphere OS:** Um sistema operacional Linux personalizado para IoT focado em segurança.
    3. **Azure Sphere Security Service:** Serviço em nuvem que monitora os dispositivos, confia neles e envia atualizações de segurança contínuas (OS e certificados).

---

## 📊 Tabela de Comparação Rápida (Para Revisão)

|**Serviço**|**Modelo**|**Melhor caso de uso (Quando escolher?)**|**Palavras-chave na Prova**|
|---|---|---|---|
|**IoT Hub**|PaaS|Precisa de controle total da arquitetura e tem equipe de dev para criar a UI.|"Comunicação central", "PaaS", "Código customizado".|
|**IoT Central**|SaaS|Quer um painel (dashboard) rápido para monitorar dispositivos sem programar.|"SaaS", "Dashboard", "Templates de indústria".|
|**Azure Sphere**|Hardware + OS|O requisito número um do cenário é **segurança** de ponta a ponta.|"Microcontrolador", "Linux seguro", "Segurança de ponta a ponta".|

---

> [!warning] Dica de Ouro para a AZ-900
> 
> - Se a questão mencionar **"painel"** ou **"interface visual"** rápida, a resposta é **IoT Central**.
>     
> - Se a questão pedir apenas o serviço de **"mensageria"** ou comunicação massiva, a resposta é **IoT Hub**.
>     
> - Se a questão grifar a palavra **"segurança profunda"**, **"hardware"** ou **"OS seguro"**, vá direto no **Azure Sphere**.
>     
